<template>
<header >
  <div class="header">
    <div class="logo-and-name">
      <img src="../assets/pinterest-social-logo.svg">
      <span class="name-company">
        <span class="red">Б</span>юро помощи призывникам
        <span class="info-company" >Юридическая помощь призывникам</span>
      </span>
    </div>

      <div class="header-call">

        <img src="../assets/call-header.svg" height="32px" width="32px" >
        <div class="header-call-info">
          <a href="tel:+79301555530" > 8 930 155 55 30 </a>
          <p>Бесплатная консультация с юристом</p>
        </div>

      </div>
      <div class="location">
            <div class="location-header">
              <img src="../assets/map.svg" height="24px" width="24px">
              <p>Тверь</p>
            </div>
            <a href="#" class="office-on-map">Наш офис на карте</a>
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



.header{
  height:100px;
  width:80%;
  display:flex;
  justify-content: space-between;
  margin:auto;

}
.logo-and-name{
  display:flex;
  margin-top:auto;
  margin-bottom:auto;

}

.logo-and-name img{
  margin-right:20px;
}
.name-company {
  display:block;
  margin-top:auto;
  margin-bottom:auto;
  font-size:18px;
}
.info-company{
  display:block;
  color:#787d88;
}
.red {
  color:red;
}


.header-call {
  display:flex;
  font-weight:300;
  margin-top:auto;
  margin-bottom:auto;
}
.header-call img{
      border-style: none;
}
.header-call a{
  color:#000;
  font-size:22px;

}

.header-call p{

  font-size:14px;
  color:#787d88;
}

.header-call-info {
  margin-left:15px;

}

.location{

  margin-top:auto;
  margin-bottom:auto;
}


.location-header{
    display:flex;
}
.location-header p{
  font-size:24px;
  margin-left:10px;
}
.office-on-map{
  color:#787d88;
  font-size:14px;
}


</style>
