<template>
<div>
  <div class="first-block">
    <div class="container">
      <div class="purple__text-image">
        <div class="purple__text">
          <PurpleEyeText class="first-block__logo" ></PurpleEyeText>
        </div>
        <nav class="purple__menu">
          <ul class="purple__menu-list">
            <li class="purple__menu-link"><a href="#">Главная</a></li>
            <li class="purple__menu-link"><a href="#">О нас</a></li>
            <li class="purple__menu-link"><a href="#">Контакты</a></li>
            <li class="purple__menu-link"><a href="#">Работы</a></li>
          </ul>
        </nav>
      </div>
    </div>
  </div>
</div>
</template>

<script>

import PurpleEyeText from "@/components/purpleEyeText";
export default {
  name: "mainPanel",
  components: {PurpleEyeText}
}
</script>

<style scoped>
a {
  text-decoration: none;
}

ul, li {
  list-style: none;
}
.first-block {
  background-color: #000;
  position: relative;
  height: 100vh;
}

.purple__text-image{
  width: 100%;
  /*position: fixed;*/
  left: 0;
  display: flex;
  overflow: hidden;

}
.purple__text{
  display: block;
  width: 100%;
}

.first-block__logo {
  width: 100%;
  max-width: 500px;
  position: absolute;
  top: -60px;
}

.purple__menu-list {
  display: flex;
  flex-wrap: nowrap;
  width: 100%;
  max-width: 800px;
  margin: 60px 0 0 0;
}

.purple__menu-link {
  display: block;

  font-size: 25px;

  margin-right: 20px;

  position: relative;

}

.purple__menu-link a {
  white-space: nowrap;
  display: block;
  color: #CE33EB;
  padding: 10px 0 10px 0;
  position: relative;

  transition: color .3s linear;
}

.purple__menu-link a:hover {
  color: #fff;
}

.purple__menu-link a:hover:after {
  content: '';
  display: block;
  position: absolute;
  left: 0;
  bottom: 0;
  height: 3px;
  width: 100%;
  background: #CE33EB;
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

@media (max-width: 1024px) {
  .first-block__logo {
    max-width: 400px;
  }
  .purple__menu-list {
    max-width: 500px;
    margin: 50px 0 0 0;
  }
  .purple__menu-link {
    font-size: 20px;
    margin-right: 15px;
  }
}

@media (max-width: 770px) {
  .first-block__logo {
    max-width: 100px;
  }
  .purple__menu-list {
    max-width: 400px;
    margin: 50px 0 0 0;
  }
  .purple__menu-link {
    font-size: 15px;
    margin-right: 10px;
  }

}
</style>