<template>
  <div class="container">
    <p class="container-header">За год вы можете ...</p>
    <div class="possibilities">

      <div class="possibility">
        <p class="possibility-header">Открыть своё собсвтенное дело</p>
        <img src="../assets/workplace.jpg" >
      </div>

      <div class="possibility">
        <p class="possibility-header">Пройти курсы и получить новую профессию</p>
        <img src="../assets/work.jpg" >
      </div>

      <div class="possibility">
        <p class="possibility-header">Привезти себя в идеальную физическую форму</p>
        <img src="../assets/running.jpg" >
      </div>

      <div class="possibility">
        <p class="possibility-header">Выучить новый язык</p>
        <img src="../assets/english.jpg" >
      </div>

    </div>






  </div>
</template>


<script>
export default {
  name: 'possibilities'
}
</script>


<style scoped>

.container
{
  margin:80px 0;
  padding:40px 0;
}
.container-header
{
  font-family: Open_Sans_Bold;
  font-size:50px;
  text-align:center;
  color:#1f1f1f;
  margin-bottom:40px;
}

.possibilities
{
  display:flex;
  justify-content:center;
  flex-wrap:wrap;
}

.possibility
{
  font-family: Open_Sans_Bold;
  font-size:25px;
  color:#047806;
  margin:10px;

}

.possibility img {
    border:2px solid black;
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
