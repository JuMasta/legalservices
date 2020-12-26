<template>
  <div id="chat" >

        <div id="chat-communication"  v-bind:style="{ visibility: visibleChat === true ? 'visible' : 'hidden' }">

          <div id="header">
            <div id="close-chat-container">
              <img id="close-chat" v-on:click="changeChatState" src="../assets/close.svg" height="20px" width="20px">
            </div>
            <div id="chat-header">
              <span id="red">Б</span>юро помощи призывникам
            </div>
            <div id="header-description">
              Ответим на любой Ваш вопрос!
            </div>
          </div>
          <div id="message-area" >
            <div class="message" v-bind:class="{ client :message.author === 'client',consultant:message.author === 'consultant'}" v-for="message in messages" :key="message.id">
                <div class="message-content">

                      {{message.text}}

                  <!-- {{message.time}} -->
                </div>
            </div>

          </div>
          <div id="input-message">
            <textarea id="text-area" v-model="message" placeholder="Впишите Ваш вопрос сюда">
              </textarea>
              <img id="send-icon" v-on:click="sendMessage"  src="../assets/right-arrow.svg" height="25px" width="50px">
          </div>

        </div>
        <img id="chat-icon" v-on:click="changeChatState"  src="../assets/chat.svg" height="100px" width="150px">



 </div>
</template>


<script>
export default {
  name: 'Chat',
  props:{
    messages:Array
  },
  // computed:{
  //   formatedMessage:function()
  //   {
  //     // return this.messages.map( item => {
  //     //   let time;
  //     //   time = item.time;
  //     //   item.time = time.getHours()
  //     //    + ':' + time.getMinutes();
  //     //   return item ;
  //     // })
  //   }
  // },
  data:function()
  {
    return {
      visibleChat:false,
      message:''
    }
  },
  methods:{
    changeChatState:function()
    {
      this.visibleChat = !this.visibleChat;
    },
    sendMessage:function()
    {

      let message = this.message;
      this.message = '';
      var request = fetch('http://localhost:8082/sendMessage',{
         method: 'GET',
         headers:
         {
           'Content-Type': 'application/json'
         },
        body: JSON.stringify({
          message:message,
          author:"client"
        })
      });
      // response.then()
      // let array = await response.json();
      // console.log(array);
      // this.messages.push(array);
      request.then(
        (response) => {
          response.json().then((data) =>{
            this.messages.push(data);
          })
        }
      )
    }
  }
}
</script>


<style scoped>

.message {
  margin-bottom:15px;
  width:100%;

}

.message-content{
    padding:10px 20px;
    max-width: 80%;
    display: inline-block;
    font-size: 17px;
    text-align: left;
    font-family: Open_Sans_Regular;

}
.client .message-content{
  background-color:#7dcdff;
  border-radius: 20px 20px 0 20px;
}
.consultant .message-content{
  background-color:#7aff85;
  border-radius: 20px 20px 20px 0;
}
.client{
  text-align:right;
  color: #2a4e7f;
  word-break: break-word;
}

.consultant{

  text-align:left;
  color: #2c633b;
}

#message-area {
  height:calc(100% - 190px);
  color:black;
  overflow-y:scroll;
  font-size:20px;
  padding: 16px 31px 16px 31px;
}

#text-area{
  height:80%;
  width:80%;
  line-height:1.5;
  font-size:15px;
  outline: none;
  resize: none;
  padding:7px 5px;
}

#send-icon{
  cursor:pointer;
}

#input-message
{
  display:flex;
  justify-content:center;
  align-items:center;
  border-top:0.5px solid #bdbdbd;
  padding:5px;
  height:80px;
  font-family: Open_Sans_Regular;
}


#header-description
{
  color:black;
  text-align:center;
  font-size:20px;
}

#close-chat-container {
  display:flex;
  justify-content: flex-end;
}

#close-chat{
  cursor:pointer;
  margin-right:15px;
  margin-top:15px;
}
#header
{
    padding-bottom:20px;
    box-shadow:0 4px 2px -2px gray;
    height:110px;
}

#red {
  color:red;
}

#chat{
  position:fixed;
  bottom:20px;
  right:20px;
  border-radius:30px;
  color:#f5f5f5;
  font-size:25px;

}
#chat-icon{
  cursor:pointer;
  position:relative;
  left:350px;
}

#chat-communication{

  display:block;
  background:#edf0f0;
  width:550px;
  height:550px;
  border-radius:30px;

}
#chat-header{
  color:black;
  font-family: Open_Sans_Regular;
  margin-bottom:10px;
}

#red{
  color:red;
}
#chat-header{
  font-size:25px;
  font-family:Open_Sans_Bold;
  text-align:center;
}

@font-face{
  font-family: Open_Sans_Light;
  src: url("../fonts/Open_Sans/OpenSans-Light.ttf");
}
@font-face {
  font-family: Open_Sans_Bold;
  src: url("../fonts/Open_Sans/OpenSans-Bold.ttf");
}
@font-face{
  font-family: Open_Sans_Regular;
  src: url("../fonts/Open_Sans/OpenSans-Regular.ttf");
}

</style>
