<script setup>
import From from './components/Form.vue'
</script>

<template>
  <!-- Form Component -->
  <From />

  <header>
    <div id="logo" onclick="slowScroll('#top')">
      <span>Overplan</span>
    </div>
    <div id="about">
      <a href="#" title="" onclick="slowScroll('#main')">Возможности</a>
      <a href="#" title="" onclick="slowScroll('#overview')">Преимущества</a>
      <a href="#" title="" onclick="slowScroll('#contacts')">Контакты</a>
      <a href="#" title="" onclick="slowScroll('#faq')">FAQ</a>
      <a href="" data-bs-toggle="modal" data-bs-target="#exampleModal" class="zakaz">Заказать проект</a>
    </div>
  </header>

  <div id="top">
    <h1 class="title-company">Overplan</h1>
    <h4 class="title-description">Ваш надежный партнёр по 1С-Битрикс и Битрикс24</h4>
  </div>

  <div id="main">
    <div class="intro">
      <h2>Разрабатываем приложения для <br>
        Битрикс24!</h2>
    </div>
    <div class="text">
      <span>Разработка гибридных мобильных приложений</span><br>
      <span>Регистрация и публикация в магазинах приложений</span>
    </div>
  </div>

  <div id="main">
    <div class="intro">
      <h2>Разрабатываем и развиваем интернет-проекты!</h2>
    </div>
    <div class="text">
      <span>Разработка интернет-магазинов</span><br>
      <span>Разработка корпоративных сайтов</span><br>
      <span>Разработка сложных интернет-решений</span><br>
      <span>Сложные интеграции с 1С и другими учетными программами</span><br>
      <span>Технический аудит интернет-проектов</span>
    </div>
  </div>

  <div id="main">
    <div class="intro">
      <h2>Внедряем, интегрируем и дорабатываем Битрикс24!</h2>
    </div>
    <div class="text">
      <span>CRM-маркетинг</span> <br>
      <span>Внедрение Битрикс24 "в коробке" для компаний от 12 сотрудников за 50 рабочих дней!</span><br>
      <span>Внедрение Битрикс24 для компаний от 12 сотрудников за 40 рабочих дней!</span><br>
      <span>Внедрение сквозной аналитики в Битрикс24!<br></span>
    </div>
  </div>

  <div id="overview">
    <h2>Преимущества</h2>
    <h4>С нами всё проще!!!</h4>

    <div class="img">
      <img src="https://avatars.mds.yandex.net/i?id=d6bca8571052140f90e8c3bb0747429dd1d409da-7092330-images-thumbs&n=13"
           alt="">
      <span>Золотой сертифицированный партнёр 1С-Битрикс</span>
    </div>
    <div class="img">
      <img src="https://cdn-ru.bitrix24.by/b15110640/landing/f61/f61924f6485a8d853919ec4d304a0cc9/bitrix24-partner_2x.png" alt="">
      <span>Золотой партнер Битрикс24 </span>
    </div>
    <div class="img">
      <img
        src="https://sun6-20.userapi.com/s/v1/if1/vSEmNP3NcS-h4vYrobfiHItSgCZ-pJR_ydq-FvbUQBtaamR-8BjhARNU7jj0GnS5XqLjDaYR.jpg?size=890x892&quality=96&crop=306,49,890,892&ava=1"
        alt="">
      <span>Интеграция с 1С</span>
    </div>
    <div class="img">
      <img src="https://wpsgroup.ru/upload/bitrix_kachestvo.png" alt="">
      <span>Участник программы качества внедрений</span>
    </div>

    <div id="contacts">
      <center><h3>Контакты</h3></center>
      <h5>Пока вы думаете,
        ваши конкуренты уже звонят нам
        и привлекают новых клиентов!</h5>
      <span>8 (800) 707-40-43</span>
      <span>hello@overplan.ru</span>
      <span>Адрес: Ярославль, ул. Угличская 39В (Здание 3), офис 204, 205</span>
      <span><p>Официальный сайт:<a href="https://overplan.ru/" style="text-decoration: none"> Overplan</a></p></span>
    </div>

    <div id="faq">
      <div>
        <span class="title">Гарантия на разработки</span><br>
        <span class="heading">Гарантийная техническая и консультационная поддержка после каждого блока работ.</span>
      </div>
      <div>
        <span class="title">Выстроенные системы</span><br>
        <span class="heading">Контроль версий, автоматический мониторинг проектов и другие технические решения.</span>

      </div>
      <div>
        <span class="title">Ответственность за результат</span><br>
        <span class="heading">Выслушиваем, высказываем экспертное мнение, разрабатываем технические задания.</span>
      </div>
    </div>
  </div>
</template>

<style scoped>
@import url(https://fonts.googleapis.com/css?family=Open+Sans);

*{
  margin: 0;
  padding: 0;
  outline: none;
}

body, html{
  width: 100%;
  height: 100%;
}

body{
  background-color: #f0f2f2;
  font-family: Trebuchet MS, Helvetica;
}

header{
  width: 100%;
  padding: 10px 0.5% 0px 0.5%;
  background: transparent;
  float: left;
  position: fixed;

}

header #logo {
  color: #fff;
  cursor: pointer;
}

header #logo span {
  font-size: 1.7em;
  line-height: 45px;
  margin-left: 40px;
  font-family: 'Suez One', serif;
}

.title-company {
  font-size: 96px;
}

.title-description {
  font-size: 52px;
}

@media (min-width: 701px) {
  #logo {
    float: left;
    width: 30%;
    font-size: 1.1em;
  }
  #about {
    float: right;
    width: 67%;
  }
}

@media (max-width: 700px) {
  #logo {
    margin-top: 15px;
    width: 100%;
    font-size: 1.5em;
  }
  #about {
    float: left;
    width: 100%;
  }
}

#about {
  text-align: center;
  font-size: 1em;
  line-height: 40px;
  margin-bottom: 10px;
}

#about > a {color: #fff}

#about > a:hover {
  color: #b0b0b0;
  text-decoration: underline;
}

#about > a:not(:last-child){
  margin-right: 7%;
}

.fixed {
  z-index: 5000;
  background-color: #fff;
  border-bottom: 1px solid silver;
}

header.fixed #logo {
  color: #343434;
}

.fixed #about a {color: #343434}
.fixed #about a:hover {color: #7c7c7c}

.zakaz {
  padding: 5px 9px;
  font-size: 1.2em;
  cursor: pointer;
}

#top {
  width: 100%;
  height: 800px;
  background-image: url(https://avatars.mds.yandex.net/i?id=5389c9b27cbea12859ddefa8e8fb9ff08566ca73-9148863-images-thumbs&n=13);
  background-blend-mode: multiply;
  background-color: #333;
  background-size: cover;
  text-align: center;
  color: #fff;
  font-size: 3em;
  vertical-align: top;
  border-radius: 0 0 30px 30px;;
}

@media (min-width: 1001px){
  #top {
    font-size: 3em;
  }
}

@media (max-width: 1000px) and (min-width: 651px){
  #top {
    font-size: 2em;
  }
}
@media (max-width: 650px){
  #top {
    font-size: 1.2em;
    padding-top: 50%;
  }
}

#top h1 {
  padding-top: 10%;
  color: #FFDEAD;
}

#top h4 {
  color: white;
  font-size: 52px;
  margin-top: 10px;
}

#main {
  float: left;
  background-color: #f6f6f6;
  border-top: 2px solid silver;
  color: black;
  font-size: 1.1em;
  border-radius: 15%;
  width: 100% !important;
}

.text {
  line-height: 35px;

}

@media (min-width: 1401px) {
  #main {
    padding: 90px 20%;
    width: 60%;
  }
}

@media (max-width: 1400px) {
  #main {
    padding: 100px 10%;
    width: 80%;
  }
}

@media (max-width: 700px){
  #main div {
    width: 98%!important;
    margin-bottom: 20px;
  }
}

#main div {
  width: 48%;
  margin-right: 2%;
  float: left;

}

#main h2 {
  font-size: 2.5em;
  text-align: left;

}
#main span {
  color: #a3a0ad;
}

#main img {
  width: 250px;
  height: 200px;
  float: left;
  padding: 10px 80px 18px 100px;
}

#overview {
  float: left;
  background-blend-mode: multiply;
  background-color: #f0f7f7;
  background-size: cover;
  background-attachment: fixed;
  width: 100%;
  text-align: center;
  color: black;
  border-radius: 8%;

}

#overview h2 {font-size: 4em}
#overview h4 {
  color: #424040;
  font-size: 3em;
  margin-top: 10px;
}

#overview p {
  text-align: left;
  font-size: 1.3em;
  margin-top: 10px;
  margin-left: 25px;
  font-family: 'Open+Sans', serif;
}


#overview .img {
  float: left;
  width: 30%;
  margin-right: 5%;
  margin-top: 50px;
  margin-bottom: 30px;
}

#overview .img:nth-child(odd) {
  margin-left: 18%;
}

#overview img {
  background: #fafafa;
  padding: 5px;
  border: 2px solid silver;
  float: left;
  width: 100%;
  max-width: 500px;
  height: 300px;
}



#overview span {
  float: left;
  width: 100%;
  font-size: 1.6em;
  margin-top: 10px;
  font-family: 'Open+Sans', serif;
}

@media (max-width: 700px) {
  #overview .img {
    width: 80%!important;
    margin-right: 0!important;
    margin-left: 10%!important;
  }
}

#contacts {
  width: 100%;
  float: left;
  padding-bottom: 40px;
  padding-top: 70px;
  border-top: 4px solid #ccc;
  background: #f4f4f4;
  border-radius: 8%;
}

h1, h2, h3, h4, h5, h6 {
  font-family: 'Open+Sans', serif;
  font-weight: lighter;
}

#contacts h3 {font-size: 3em; color: #4f4f4f}

#contacts h5 {
  font-size: 1.5em;
  color: #8c8f8f;
  margin-top: 10px;
}

#contacts span {
  color: black;
}

#contacts span> p {
  color: #8c8f8f;
  text-align: center;
  font-size: 1em;
}


#faq {
  background-color: #fff;
  border-top: 2px dashed #e4e3e3;
  width: 100%;
  float: left;
  padding-top: 70px;
  padding-bottom: 70px;
}

#faq div {
  width: 25%;
  margin-left: 6%;
  float: left;
}

@media (min-width: 801px) {
  #faq div {
    width: 25%;
    margin-left: 6%;
    float: left;
  }
}

@media (max-width: 800px) {
  #faq div {
    width: 80%;
    margin-left: 10%;
    float: left;
  }
}

#faq .title {
  font-weight: lighter;
  color: #a3a0ad;
  margin-bottom: 20px;
  font-size: 2.2em;
  text-align: left;
}

#faq .heading {
  color: #7d7d7d;
  font-size: 1.3em;
  font-weight: bold;
  text-align: left;
}
</style>
