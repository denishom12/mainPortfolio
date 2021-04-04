<template>
  <div class="mail">
    <section id="contact">
      <div class="container__feed-back">
        <div class="feed__back">
          <div class="headInfo">
            <div class="head">
              <p class="title">Свяжитесь с нами <br>для сотрудничества</p>
              <p class="line"></p>
              <p class="subtitle">
                Воспользуйтесь формой ниже, или отправьте письмо по нашему адресу<br>
                <span class="ourMail">
                PurpleEyeStudio@hotmail.com
              </span>
              </p>
            </div>
          </div>
          <div class="cont">
            <form class="contactForm" action=”mailto:purpleeyestudio@hotmail.com” method="post" enctype=”multipart/form-data” name=”EmailForm”>
              <input placeholder="<Имя>" name="name" type="text" required>
              <input placeholder="<Email>" name="email" type="text" required>
              <textarea placeholder="<Сообщение>" name="message" type="text"></textarea>
              <button id="submit" type="submit">Отправить</button>
            </form>
          </div>
        </div>
      </div>
    </section>

  </div>
</template>

<script>
export default {
  name: "mail"
}
</script>

<style scoped>
.mail{
  background-color: black;
  height: 120vh;
}
#contact {
  display: flex;
  flex-direction: column;
  justify-content: center;
  width: 100%;
  height: 100vh;
}

.container__feed-back {
  width: 85%;
  max-width: 1300px;
  margin: 0 auto;
}

.feed__back {
  width: 100%;
  max-width: 880px;
  margin: 0 auto;
}

.title{
  font-size: 3em;
  color: white;
}

.subtitle{
  font-size: 1em;
  color: white;
}

.line{
  background: #f300b4;
  width: 200px;
  height: 3px;
  margin: 1rem 0;
}

.contactForm{
  display: flex;
  flex-direction: column;
  align-items: center;
  width: 100%;
  margin-top: 1rem;
}

.contactForm input[type="text"],input[type="email"], textarea{
  border-bottom: 2px solid white;
  background: transparent;
  color: white;
  font-size: 1.8rem;
}

.contactForm textarea {
  resize: none;
  border-bottom: 2px solid white;
}

.contactForm input{
  border: none;
  padding: 1rem;
  font-family: 'Overlock', Arial, Helvetica, sans-serif;
  width: 100%;
  height: 40%;
}

.contactForm button{
  padding: 1rem;
  font-family: 'Overlock', Arial, Helvetica, sans-serif;
  height: 40%;
  margin-top: 30px;
  background-color: #f300b4;
  align-self: flex-end;
  font-size: 25px;
}

.cont form input[type="text"]:hover,input[type="email"]:hover, textarea:hover{
  border-bottom: 3px solid #f300b4;
  background: transparent;
  color: white;
  font-size: 1.8rem;
  box-shadow: none;
  outline: none;
}

.contactForm textarea{
  padding: 1rem;
  font-family: 'Overlock', Arial, Helvetica, sans-serif;
  width: 100%;
  height: 40%;
  overflow: auto;
  outline: none;
  border-left: none;
  border-right: none;
}

input[type="submit"]{
  background: #f300b4;
  color: white;

  width: auto;
  float: right;
}


@media (max-width: 804px) {
  .title{
    font-size: 2.8em;
    color: white;
  }
  .contactForm input[type="text"],input[type="email"], textarea{
    font-size: 1.5rem;
  }
  .contactForm button{
    padding: 1rem;
    font-family: 'Overlock', Arial, Helvetica, sans-serif;
    height: 2%;
    margin-top: 30px;
    background-color: #f300b4;
    align-self: flex-end;
    font-size: 16px;
  }
}
@media (max-width: 750px) {
  .title{
    font-size: 2.6em;
    color: white;
  }
  .contactForm input[type="text"],input[type="email"], textarea{
    font-size: 1.4rem;
  }
}

@media (max-width: 700px) {
  .title{
    font-size: 2.2em;
    color: white;
  }
  .contactForm input[type="text"],input[type="email"], textarea{
    font-size: 1.2rem;
  }
}
@media (max-width: 592px) {
  .title{
    font-size: 2em;
    color: white;
  }
  .contactForm input[type="text"],input[type="email"], textarea{
    font-size: 1rem;
  }
}

@media (max-width: 538px) {
  .title{
    font-size: 1.8em;
    color: white;
  }
}
@media (max-width: 486px) {
  .title{
    font-size: 1.3em;
    color: white;
  }
  .contactForm button{
    align-self: center;
  }
}
@media (max-width: 354px) {
  .title{
    font-size: 1em;
    color: white;
  }
}
input::-moz-placeholder { color: white; }
input::-webkit-input-placeholder { color: white;}
textarea::-moz-placeholder { color: white; }
textarea::-webkit-input-placeholder { color: white; }
</style>