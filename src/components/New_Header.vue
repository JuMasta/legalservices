<template>
<header >
  <div id="main-header">
    <div id="main-header-container">
      <div id="navigation">
        <ul id="nav-list">
            <li><a>О компании</a></li>
            <li class="li-margin"><a>Советы юриста</a></li>
            <li class="li-margin"><a>Контакты</a></li>
            <li class="li-margin"><a>Наш адрес на карте</a></li>
        </ul>
      </div>
      <div id="location">
        <img src="../assets/location.svg" height="18px" width="20px" >
        <span>Ваш город: </span>
        <a id="cityLink">Тверь</a>
      </div>
    </div>
  </div>

  <div id="info-header">
    <div id="info-header-container">
    <div id="company-name">
      <div id="name"><span id="red">Б</span>юро помощи призывникам</div>
      <span id="company-services" >Юридическая помощь призывникам</span>
    </div>
    <div id="call-info">

      <img src="../assets/call-header.svg" height="32px" width="32px" >
      <div id="header-call-info">
        <a href="tel:+79301555530" > 8 930 155 55 30 </a>
        <p>Бесплатная консультация с юристом</p>
      </div>

    </div>
  </div>
</div>

    <div id="info-nav-header">
      <div id="info-nav-header-container">

        <div id="services">
          <ul id="list-services">
            <li>

              <a class="underline" href="#" >как мы будем работать с вами?</a>
            </li>
            <li class="li-margin-service">
              <a class="underline" href="#" >адрес на карте</a>
            </li>
            <li class="li-margin-service">
              <a class="underline" href="#" >цены</a>
            </li>
            <li class="li-margin-service">
              <a class="underline" href="#" >консультация</a>
            </li>
          </ul>
        </div>
        <div id="contacts">

            <span>Можем подробно рассказать всё тут</span>
            <a href="#"><img src="../assets/telegram.svg" height="25px" width="25px" ></a>
            <a href="#"><img src="../assets/instagram.svg" height="25px" width="25px" ></a>
            <a href="#"><img src="../assets/vk.svg" height="25px" width="25px" ></a>
            <a href="#"><img src="../assets/whatsapp.svg" height="25px" width="25px" ></a>

        </div>

      </div>
    </div>

</header>
</template>


<script>
export default {
  name: 'Header'
}
</script>


<style scoped>


Header{
    font-family: Open_Sans_Light;
}
#main-header {

  background-color:#0a0f1b;
  color:#919191;
  padding:6px 0;

}
#main-header-container{
  display:flex;
  justify-content:space-between;
  padding:0 30px;
  max-width: 1170px;
  min-width: 320px;
  margin: 0 auto;
}
.li-margin{
  margin-left:70px;
}
.li-margin-service{
  margin-left:40px;
}
#nav-list li{
  display:inline;

}
#location img {
  position:relative;
  top:1.5px;
  margin-right:5px;
}
#cityLink{
    color:#fff;
}
#info-header{

  border-bottom:0.5px solid #b3b3b3;
}
#info-header-container{
  display:flex;
  justify-content:space-between;
  padding:30px 70px;
  max-width: 1170px;
  min-width: 320px;
  margin: 0 auto;

}
#red{
  color:red;
}
#name{
  font-size:25px;
  font-family:Open_Sans_Bold;
}
#company-services{
  display:block;
  text-align:center;
  font-size:16px;
  font-family:Open_Sans_Bold;
  color:#787d88;
}
#call-info {
  display:flex;
  font-weight:300;
  margin-top:auto;
  margin-bottom:auto;
  font-family:Open_Sans_Bold;
}
#call-info img{
      border-style: none;
}
#call-info a{
  color:#000;
  font-size:22px;

}

#call-info p{

  font-size:14px;
  color:#787d88;
}
#header-call-info{
  margin-left:20px;
}
#info-nav-header-container{
  display:flex;
  justify-content:space-between;
  width:90%;
  padding:20px 30px;
  margin: 0 auto;

}
#list-services li{
  display:inline;
  font-family: Open_Sans_Bold;
  font-size:18px;
}
.underline  {
  color:#000;
  transition: border 0.3s linear; /*задаём время анимации*/
}
.underline:hover{
  border-bottom:4px solid red;
}


#contacts span{
  font-family: Open_Sans_Regular;
  font-weight:150;
  margin-right:5px;
}
#contacts a{
  margin-left:5px;
  margin-right:5px;
  position:relative;
  top:4px;

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
