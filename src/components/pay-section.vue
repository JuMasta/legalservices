<template>
<div class="container">
  <p class="section-header" >Выбирайте надёжных партнёров </p>
  <div class="conditions">

    <div class="condtition">
    <div class="img-background">
      <img src="../assets/contract.png" >
    </div>
    <div class="text-condition">
      <p>Всё по договору!</p>
    </div>
    <div class="description-condition">
      Заключим с вами официальный договор оказания услуг. Вы будете защищены законом “О защите прав потребителей”.
    </div>
    </div>

    <div class="condtition">
    <div class="img-background">
      <img src="../assets/coins.png" >
    </div>
    <div class="text-condition">
      <p>Рассрочка платежа!</p>
    </div>
    <div class="description-condition">
      Наши услуги можно оплачивать в рассрочку до 12 месяцев без участия банков. Платежи от 4100 руб./месяц в зависимости города.
    </div>
    </div>

    <div class="condtition">
    <div class="img-background">
      <img src="../assets/clock.png" >
    </div>
    <div class="text-condition">
      <p>В короткие сроки!</p>
    </div>
    <div class="description-condition">
      Комплекс наших услуг направлен на скорейшее достижение результата, на которое в среднем требуется 1-2 призыва.
    </div>
    </div>

    <div class="condtition">
    <div class="img-background">
      <img src="../assets/money-back.png" >
    </div>
    <div class="text-condition">
      <p>Вернём деньги!</p>
    </div>
    <div class="description-condition">
      Если мы не сможем вам помочь, вернем вам 100% нашего гонорара. Данное условие прописано в договоре.
    </div>
    </div>

  </div>
</div>
</template>


<script>
export default {
  name: 'PaySection'
}
</script>


<style scoped>

.container{

  padding-top:30px;
  padding-bottom:30px;
  margin:80px 0;



}
.conditions {
  margin-top:80px;
  display:flex;
  justify-content:space-around;
}
.condtition
{


  padding-left:10px;
  padding-right:20px;

}
.img-background{
  background:#ff1818;
  height:180px;
  width:200px;
  padding:20px;
  border-radius:50%;
  text-align:center;
}
.section-header{
  display:block;
  font-size:50px;
  font-family: Open_Sans_Bold;
  text-align:center;


}
.text-condition{
    margin-top:20px;
    margin-bottom:20px;
    font-family: Open_Sans_Bold;
    color:#000;
    font-size:20px;


}
.text-condition p{
  border-radius:3px;

}
.description-condition {
  font-family: Open_Sans_Regular;
  font-size:17px;
  max-width:250px;
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
