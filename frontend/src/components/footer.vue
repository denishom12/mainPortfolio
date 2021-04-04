<template>
  <div>
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <div class="footer">
      <div class="footer__pes">
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
  height: 100vh;
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
  position: relative;
  justify-content: space-around;
  width: 56em;
  margin-top: 1%;
}
.footer__name h1{
  font-size: 6.8em;
  color: white;
  margin-top: 20%;
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
  margin-right: -13em;
}
.footer__group{
  color: white;
  margin-right: 13em;
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
}
.copyright__text1{
  color: white;
  font-size: 1em;
}
@media (max-width: 1500px) {
  .footer__name h1{
    margin-top: 0%;
    font-size: 7em;
  }
}
@media (max-width: 900px) {
  .footer__name h1{
    font-size: 4em;
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
  .footer__contain{
    flex-direction: column;
    align-items: center;
    justify-content: space-around;
  }
}
@media (max-width: 858px) {
  .footer__name h1{
    font-size: 4em;
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
    font-size: 4em;
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
@media (max-width: 508px) {
  .footer__name h1{
    font-size: 3.5em;
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
    font-size: 3em;
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
    font-size: 2.6em;
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
}
@media (max-width: 384px) {
  .footer__name h1{
    font-size: 2.5em;
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

