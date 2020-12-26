<template>
  <div class="container">
    <p class="section-header">5 шагов по получению военного билета:</p>

    <div class="content">
        <div class="steps">
          <div class="step">
            <div class="step-number">
              <p>1 ШАГ</p>
            </div>
            <div class="step-icon">
              <img  height="200px" width="200px" src="../assets/consultation.svg" >
            </div>
            <div class="step-descrition">
              <p class="title-description">Бесплатная консультация</p>
              <p class="text-description">Запишись на бесплатную юридическую консультацию – очно или дистанционно. На ней юрист изучит твою ситуацию, правовой статус, а затем  расскажет о законных методах решения твоей проблемы</p>
            </div>
          </div>


          <div class="step">
            <div class="step-number">
              <p>2 ШАГ</p>
            </div>
            <div class="step-icon">
              <img  height="200px" width="200px" src="../assets/agreement.svg" >
            </div>
            <div class="step-descrition">
              <p class="title-description">Гарантия</p>
              <p class="text-description">Мы приступаем к оформлению договора, который гарантирует 100% законность и исполнение наших обязательств, а также возврат средств, если тебя все-таки заберут в армию. Мы также подписываем нотариальную доверенность, которая гарантирует защиту твоих интересов в суде, военном комиссариате или сборном пункте в день «Х»</p>
            </div>
          </div>

          <div class="step">
            <div class="step-number">
              <p>3 ШАГ</p>
            </div>
            <div class="step-icon">
              <img  height="200px" width="200px" src="../assets/search.svg" >
            </div>
            <div class="step-descrition">
              <p class="title-description">Изучение личного дела</p>
              <p class="text-description">Юрист приступает к изучению твоего личного дела. Наши врачи направят тебя на независимое обследование для выявления заболеваний, которые могут освободить тебя от призыва.</p>
            </div>
          </div>

          <div class="step">
            <div class="step-number">
              <p>4 ШАГ</p>
            </div>
            <div class="step-icon">
              <img  height="200px" width="200px" src="../assets/document.svg" >
            </div>
            <div class="step-descrition">
              <p class="title-description">Готовим пакет документов</p>
              <p class="text-description">Параллельно мы готовим пакет документов. Инструктируем тебя к походу в военкомат, где необходимо пройти проверку диагноза. После его подтверждения, ты получаешь в военном комиссариате непризывную категорию годности и военный билет.</p>
            </div>
          </div>

          <div class="step">
            <div class="step-number">
              <p>5 ШАГ</p>
            </div>
            <div class="step-icon">
              <img  height="200px" width="200px" src="../assets/battle.svg" >
            </div>
            <div class="step-descrition">
              <p class="title-description">Бьемся за вас</p>
              <p class="text-description">Альтернативный сценарий: если военкомат все равно признает тебя годным, в дело вступает юрист. Он будет оспаривать неправомерное решение призывной комиссии в судебном и досудебном порядке до последнего – получения законной отсрочки или освобождения от армии</p>
            </div>
          </div>
        </div>
    </div>
  </div>
</template>


<script>
export default {
  name: 'zakonadatelstvo'
}
</script>


<style scoped>

.container{
  margin:80px 0;
  padding:40px 0;
  background-size:cover;

}

.section-header{
  display:block;
  font-size:35px;
  font-family: Open_Sans_Bold;
  text-align:center;
  color:#1f1f1f;
  margin-bottom:80px;


}
.content{
  margin-top:25px;
}
.steps{
  padding:0 50px;
}
.step{
  display:flex;
  justify-content:space-around;
  padding-bottom:75px;
  border-bottom:0.2px solid #a1a1a1;
  margin-bottom:75px;

}
.step-number{
  margin-left:10px;
  margin-right:10px;
  font-family: Open_Sans_Bold;
  font-size:25px;
}
.step-icon{
  margin-left:10px;
  margin-right:10px;
}
.step-descrition{
  margin-left:10px;
  margin-right:10px;
  max-width:400px;

}
.title-description
{

  font-family: Open_Sans_Bold;
  font-size:25px;
  margin-bottom:20px;
}

.text-description
{
  font-family: Open_Sans_Regular;
  font-size:15px;
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
