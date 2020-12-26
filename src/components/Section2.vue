<template>
  <section class="section">
    <div class="wrapper">
    <h1 class="headerOfSection font-size-50">Не хотите звонить?</h1>
    <h3 class="headerInfo font-size-35">Тогда напишите нам и наш юрист развеет все ваши сомнения</h3>
    <div class="message-form">
      <form class="form">
        <p class="form-header">Онлайн консультация</p>
        <input class="message" type="textarea" placeholder="Напишите нам!"/>
        <button class="submit-message" type="submit">Задать вопрос</button>
      </form>
    </div>
  </div>
  </section>
</template>


<script>
export default {
  name: 'Section2'
}
</script>


<style scoped>

@font-face {
  font-family: Open_Sans_Bold;
  src: url("../fonts/Open_Sans/OpenSans-Bold.ttf");
}
@font-face{
  font-family: Open_Sans_Light;
  src: url("../fonts/Open_Sans/OpenSans-Light.ttf");
}
@font-face{
  font-family: Open_Sans_Regular;
  src: url("../fonts/Open_Sans/OpenSans-Regular.ttf");
}

.section{
    padding:100px;
    font-family: Open_Sans_Regular;
    text-align:center;
    background-color:#bde8ff;

    color: #707d88;
}

.headerOfSection{
    cursor:pointer;

}
.font-size-50{
  font-size:70px;
}
.font-size{
  font-size:35px;
}
.message-form {
  margin-top:30px;
  margin-left:auto;
  margin-right:auto;

  border-radius:10px;
  width:500px;
  height:400px;
}
.form-header{
  font-family: Open_Sans_Bold;
  font-size:18px;
  color:#000;
}
.wrapper{

}
.message{
  display:block;
  margin-top:10px;
  margin-left:auto;
  margin-right:auto;
  width:70%;
  height:150px;
  border-radius:10px;
  border:solid 1px #e0e0e0;
  padding:10px;
  vertical-align:top;

}
.message:focus{
 outline:none;
}
.submit-message{
  display:block;
  margin-top:10px;
  margin-left:auto;
  margin-right:auto;
  height:50px;
  width:70%;
  border-radius:10px;
  border:none;
  cursor:pointer;
  font-size:20px;
  background-color:#7fadf5;
}



</style>
