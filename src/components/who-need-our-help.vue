<template>
  <div id="container">

    <div id="content">


          <a class="situation-help">
            <h3><span class="img-svg"><img src="../assets/verified.svg?fill=#000" height="35px" width="35px" >
            </span><span>Получили повестку в военкомат для прохождения воинской службы?</span></h3>
            </a>

            <a class="situation-help">
              <h3><span class="img-svg"><img src="../assets/verified.svg?fill=#000" height="35px" width="35px" >
              </span><span>Не согласны с решением призывной комиссии?</span></h3>
              </a>

              <a class="situation-help">
                <h3><span class="img-svg"><img src="../assets/verified.svg?fill=#000" height="35px" width="35px" >
                </span><span>Хотите освободится от призыва законным путём без взяток?</span></h3>
                </a>

                <a class="situation-help">
                  <h3><span class="img-svg"><img src="../assets/verified.svg?fill=#000" height="35px" width="35px" >
                  </span><span>Чувствуете себя не готовым к армейской службе?</span></h3>
                  </a>

                  <a class="situation-help">
                    <h3><span class="img-svg"><img src="../assets/verified.svg?fill=#000" height="35px" width="35px" >
                    </span><span>Считаете , что на "Гражданке"  принесёте больше пользы стране?</span></h3>
                    </a>


    </div>

  </div>
</template>
<script>
export default
{
  name:"help"
}
</script>
<style scoped>



.situation-help{
    display:flex;
    border:2px solid #e02416;
    padding:25px 20px;
    border-radius:10px;
    font-family: Open_Sans_Light;
    margin-bottom:20px;


}
#content{
  width:100%;
  padding:0 15px;
  margin-right:auto;
  margin-left:auto;
  max-width:930px;
}
.img-svg img{
  margin-right:7px;
}
.situation-help:hover
{
  color:white;
  background:#cf4938;
  cursor:pointer;
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
