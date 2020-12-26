<template>
  <section class="section">
    <div class="content">
      <div class="col1">
        <div class="header-col1">
            Профессиональные юридические услуги призывникам
        </div>
        <div class="info-col1">
            <p>Введите ваш номер телефона и мы сами вам перезвоним
              <br>
              <strong>в течении 5 минут</strong>
            </p>
        </div>
        <ul class="list" >
          <li class="services-col1 item1">Мы оказываем успешную юридическую помощь призывникам</li>
          <li class="services-col1 item2">Мы гарантируем возврат средств в случае отрицательного результата</li>
          <li class="services-col1 item3">Мы развеем все ваши сомнения и страхи </li>
        </ul>
      </div>
      <div class="col2">
            <form>
              <div class="form-header">
                <p>Введите ваш номер телефона и мы вам перезвоним!</p>

                <div class="input-phone">
                  <img src="../assets/phone-call.svg" height="25px" width="25px" >
                  <input type="tel" class="form-input" placeholder="Введите ваш номер телефона"/>
                </div>
                <button class="form-button">Получить консультацию</button>
              </div>
            </form>
      </div>
    </div>
  </section>
</template>


<script>
export default {
  name: 'Section1'
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



.section {
  padding-bottom:50px;
  padding-top:50px;
  background: url("../assets/tabs-wrap-bg.jpg") 60% 60%;

  background-size:cover;
  background-repeat:no-repeat;


}
.content{
  display:flex;
  padding-top:70px;
  padding:10px;
  margin:auto;
  max-width:1000px;
  color:#fff;
  line-height:1.5;
  font-family:Open_Sans_Regular;
}

.header-col1 {

  font-size:25px;
  font-weight:700;
  margin-bottom:10px;
  font-family: Open_Sans_Bold;

}

.info-col1{

  font-size:15px;
  font-weight:350;
  margin-bottom:20px;


}

.services-col1{

  padding: 0 0 10px 10px;
  line-height:25px;
  font-weight:400;
  vertical-align: top;
  font-size:20px;
}
.item1{
  list-style-image:url("../assets/number1.svg");
}
.item2{
  list-style-image:url("../assets/two.svg");
}
.item3{
  list-style-image:url("../assets/three.svg");
}
.col2 form{

  background:#fff;
  border-radius:10px;
}

.form-header{

  padding:20px;
  border-radius:5px;
  border-style:none;

}
.form-header p{
  color:#000;
  font-family:Open_Sans_Bold;
  font-size:15px;
  margin-bottom:10px;
}
.input-phone {
  padding:10px;
  background-color: #f5f5f5;
  margin-bottom:20px;
  border-radius:5px;
}
.input-phone img{
  margin-right:10px;

}
.form-input{
  width:85%;
  border: none;
  background-color: transparent;
  font-size: 18px;
  color:#4287f5;

}
.form-input:focus {
    border:none;
    outline:none;
}
.form-input::placeholder{
  color:#4287f5;
}
.form-button{
  width:100%;
  height:50px;
  border-style:none;
  border-radius:5px;
  background-color:#7fadf5;
  cursor:pointer;
  font-size:16px;
  padding:10px;
  text-align:center;
}





</style>
