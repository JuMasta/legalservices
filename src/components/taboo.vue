<template>
  <div id="container">
    <div id="content">
      <div id="taboo-list">
        <div class="taboo-item">
          <div class="taboo-content">
            <img height="50px" width="50px" src="../assets/cancel.svg">
            <div class="taboo-text">
              Мы не являемся звеном коррупции, работа только в рамках закона
            </div>
         </div>
        </div>

        <div class="taboo-item">
          <div class="taboo-content">
            <img height="50px" width="50px" src="../assets/cancel.svg">
            <div class="taboo-text">
              Мы не занимаемся подделкой медицинских документов
            </div>
         </div>
        </div>


        <div class="taboo-item">
          <div class="taboo-content">
            <img height="50px" width="50px" src="../assets/cancel.svg">
            <div class="taboo-text">
              Мы не выдаем готовые военные билеты
            </div>
         </div>
        </div>
      </div>
    </div>
  </div>
</template>


<script>
  export default {
    name:"taboo"
  }

</script>

<style scoped>

#container
{
  
  margin:50px 0;

}

#content{
  background:#e02416;
}
.taboo-content{
  display:flex;
}
#taboo-list{
  display:flex;
  justify-content:center;
  padding:30px 30px;
}
.taboo-text {
  font-size:20px;
  font-family: Open_Sans_Regular;
  color:white;
  margin-left:10px;
  max-width:250px;
}
.taboo-item
{
    margin:0 20px;
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
