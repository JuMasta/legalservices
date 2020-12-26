<template>
  <div class="main-begin">
    <div class="container">
      <div class="content-of-container">
        <span class="content-of-container-title" >Освободись от службы в армии законно</span>
        <span class="content-of-container-text">Оказываем услуги, направленные на получение военного билета или отсрочки по основаниям, предусмотренным законодательством РФ.</span>
        <div class="future-list">
          <div class="future-list-content">
             <img src="../assets/number1.svg" height="15px" width="15px" ><span class="title-span">ПРОФЕССИОНАЛЬНО</span>
             <span class="block-span">Помощь призывникам - единственная специализация нашей компании.</span>
          </div>
          <div class="future-list-content">
             <img src="../assets/two.svg" height="15px" width="15px" ><span class="title-span">ИНДИВИДУАЛЬНО</span>
             <span class="block-span">Осуществляем полное сопровождение на всех этапах работы.</span>
          </div>
          <div class="future-list-content">
             <img src="../assets/three.svg" height="15px" width="15px" ><span class="title-span">ВОЗВРАТ</span>
             <span class="block-span">Гарантируем возврат средств в случае отрицательного результата.</span>
          </div>
        </div>
          <div  class="action-content">
            <button>Бесплатная консультация</button>
          </div>
      </div>
    </div>
  </div>
</template>


<script>
export default {
  name: 'SiteContent'
}
</script>


<style scoped>
.action-content {
  margin-top:30px;
  margin-bottom:30px;
}
.action-content button{
  box-shadow: 0 4px 0 0 #790a0a;
  font-size: 16px;
  color: #fff;
  background-color:#ff1818;
  text-transform: uppercase;
  text-align: center;
  text-shadow: 0 2px 0 rgba(0,0,0,0.2);
  padding: 21px 40px;
  border-radius: 10px;
  border: 1px solid #ff1818;
  font-weight: 700;
  word-spacing: 6px;
}
.future-list img {
  margin-right:5px;
}
.title-span{
  font-size:15px;
  font-family: Open_Sans_Bold ;
      text-transform: uppercase;
}
.block-span{
  display:block;
  font-family: Open_Sans_Regular ;

}
.future-list span {
  color:white;


}
.future-list-content{
  margin-left:15px;
  width:350px;
}
.future-list{
  display:flex;
}
.main-begin{
  padding-top: 50px;
  padding-bottom: 50px;
  background: #1a1e29 url("../assets/bg1.jpg") bottom center no-repeat;

}
.container{
  width: 100%;
  max-width: 980px;
  min-width: 320px;
  margin: 0 auto;
  padding: 25px 80px 25px 25px;
  border: 7px solid white;
}
.content-of-container-title{
  display:block;
  font-family: Open_Sans_Bold;
  color:white;
  font-size:42px;
  line-height:1.1;
}
.content-of-container-text{
  display:block;
  font-family: Open_Sans_Regular;
  font-size:16px;
  color:white;
  margin: 30px 0 30px 0;
}
@font-face{
  font-family: Open_Sans_Regular;
  src: url("../fonts/Open_Sans/OpenSans-Regular.ttf");
}
@font-face {
  font-family: Open_Sans_Bold;
  src: url("../fonts/Open_Sans/OpenSans-Bold.ttf");
}
</style>
