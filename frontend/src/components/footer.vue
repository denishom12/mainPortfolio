<template>
  <div>
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <div class="footer">
      <div class="footer__pes">
        <img class="blop__image" src="../assets/blop5.svg" alt="">
        <div class="footer__name">
          <h1>Purple eye studio</h1>
        </div>
        <div class="footer__logo">
          <div class="footer__line">
            <p ></p>
          </div>
          <div >
            <img class="footer__image" src="../assets/eyelogo3.svg" alt="">
          </div>
          <div class="footer__line">
            <p ></p>
          </div>
        </div>
      </div>
      <div class="footer__contain">
        <div class="footer__group">
          <h1 class="footer__call">Позвонить</h1>
          <p>8(999)-518-79-12</p>
          <p>8(999)-518-79-12</p>
        </div>
        <div class="footer__group">
          <h1 class="footer__message">Написать</h1>
          <p>purpleeyestudio@hotmail.com</p>
        </div>
        <div class="footer__group">
          <h1 class="footer__about">О нас</h1>
        </div>
      </div>
      <div class="footer__linker">
        <div>
          <a href=""><img class="footer__instagram" src="../assets/logoinst.png" alt=""></a>
        </div>
        <div>
          <a href=""><img class="footer__instagram" src="../assets/logoinst.png" alt=""></a>
        </div>
      </div>
      <div class="footer__copyright">
        <div>
          <h1 class="copyright__text">© PurpleEyeStudio 2021</h1>
        </div>
        <div >
          <a href=""><h1 class="copyright__text1" >Copyright</h1></a>
        </div>
        <div >
          <a href=""><h1 class="copyright__text1">Политика конфиденциальности</h1></a>
        </div>
      </div>
    </div>
  </div>
</template>

<style>
.blop__image{
  margin-top: -0.25%;
}
@media (max-width: 1820px){
  .blop__image{
    visibility: hidden;
  }
}

.footer__group p {
  white-space: nowrap;
  display: block;
  color: #fff;
  padding: 10px 0 10px 0;
  position: relative;

  transition: color .3s linear;
}

.footer__group p:hover {
  color: #f300b4
}

.footer__group p:hover:after {
  content: '';
  display: block;
  position: absolute;
  left: 0;
  bottom: 0;
  height: 3px;
  width: 100%;
  background: #f300b4;
  z-index: 1;
  animation: .2s linear line;
}

@keyframes line {
  from {
    width: 0;
  }
  to {
    width: 100%;
  }
}

.footer{
  background-color: black;
}
.footer__pes{
  display: flex;
  position: relative;
  flex-direction: column;
  align-items: center;
}
.footer__logo{
  display: flex;
  margin-top: -7%;
  position: relative;
  justify-content: space-around;
  width: 60em;

}
.footer__name h1{
  font-size: 6.8em;
  font-family: "PT Mono";
  color: white;
  margin-top: -32%;
}
.footer__image{
  width: 50%;
  margin-left: 25%;
}
.footer__line{
  background: #f300b4;
  width: 30%;
  height: 3px;
  margin-top: 7%;
}
.footer__contain{
  margin-left: 8em;
}
.footer__contain h1, p{
  font-family: "PT Mono";
}
.footer__group{
  color: white;
  margin-right: 8em;
}
.footer__linker{
  display: flex;
  position: relative;
  justify-content: center;
  align-items: center;
  margin-top: 1%;
  width: 100%;
}
.footer__instagram{
  max-width:200px;
  transition: all .3s;
}

.footer__instagram:hover{
  transform: scale(1.2);
  transition: all .3s;
}
.footer__copyright{
  display: flex;
  justify-content: center;
  margin-top: 10%;
}
.footer__copyright *{
  text-decoration: none;
}
.copyright__text{
  color: white;
  font-size: 1em;
  font-family: "PT Mono";
  margin-right: 8em;
  margin-left: 10em;
}
.copyright__text1{
  color: white;
  font-size: 1em;
  margin-right: 8em;
  font-family: "PT Mono";
}
@media (max-width: 1600px) {
  .footer__logo{
    margin-top: auto;
  }
  .footer__name h1{
    margin-top: auto;
  }
  .copyright__text{
    font-size: 1em;
    margin-right: 3em;
    margin-left: 4em;
  }
  .copyright__text1{
    font-size: 1em;
    margin-right: 4em;
  }
}
@media (max-width: 1500px) {
  .footer__name h1{
    margin-top: 0%;
    font-size: 5em;
  }
}
@media (max-width: 900px) {
  .footer__name h1{
    font-size: 3em;
  }
  .footer__logo{
    width: 32em;
  }
  .copyright__text{
    font-size: 1em;
    margin-right: 3em;
    margin-left: 4em;
  }
  .copyright__text1{
    font-size: 1em;
    margin-right: 4em;
  }
  .footer__contain{
    flex-direction: column;
    align-items: center;
    justify-content: space-around;
  }
}
@media (max-width: 858px) {
  .footer__name h1{
    font-size: 3em;
  }
  .footer__logo{
    width: 32em;
  }
  .copyright__text{
    font-size: 1em;
  }

  .copyright__text1{
    font-size: 1em;
  }
}
@media (max-width: 634px) {
  .footer__name h1{
    font-size: 3em;
  }
  .footer__logo{
    width: 32em;
  }
  .copyright__text{
    font-size: 0.4em;
    margin-right: 0em;
    margin-left: 0em;
  }
  .copyright__text1{
    font-size: 0.4em;
    margin-right: 0em;
  }
  .footer__contain h1, p{
    font-size: 1.5em;
  }
}
@media (max-width: 508px) {
  .footer__name h1{
    font-size: 2.5em;
  }
  .footer__logo{
    width: 28em;
  }
  .copyright__text{
    font-size: 0.8em;
  }
  .copyright__text1{
    font-size: 0.8em;
  }
}

@media (max-width: 450px) {
  .footer__name h1{
    font-size: 2em;
  }
  .footer__logo{
    width: 25em;
  }
  .copyright__text{
    font-size: 0.7em;
  }
  .copyright__text1{
    font-size: 0.7em;
  }
}
@media (max-width: 405px) {
  .footer__name h1{
    font-size: 1.6em;
  }
  .footer__logo{
    width: 22em;
  }
  .copyright__text{
    font-size: 0.65em;
  }
  .copyright__text1{
    font-size: 0.65em;
  }
  .footer__contain h1, p{
    font-size: 1em;
  }
}
@media (max-width: 384px) {
  .footer__name h1{
    font-size: 1.5em;
  }
  .footer__logo{
    width: 20em;
  }
  .copyright__text{
    font-size: 0.6em;
  }
  .footer__instagram{
    max-width:150px;
  }
  .copyright__text1{
    font-size: 0.6em;
  }
}
.footer__contain{
  display: flex;
  justify-content: center;
}
</style>

<script>
export default {
  name: "footer"
}
</script>

