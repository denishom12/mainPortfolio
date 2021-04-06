<template>
  <div class="home">
    <div class="home__main">
      <MainPanel></MainPanel>
    </div>
    <div class="home__sites">
      <SitePanel></SitePanel>
    </div>
    <div class="home__people">
      <PeopleOneTwo></PeopleOneTwo>
    </div>
    <div class="home__mail">
      <Mail></Mail>
    </div>
    <div class="home__footer">
      <Footer></Footer>
    </div>
  </div>
</template>

<script>

import Footer from "@/components/footer";
import Mail from "@/components/mail";
import PeopleOneTwo from "@/components/peopleOneTwo";
import SitePanel from "@/components/sitePanel";
import MainPanel from "@/components/mainPanel";

export default {
  name: 'Home',
  components: {
    MainPanel,
    SitePanel,
    PeopleOneTwo,
    Footer,
    Mail,

  }
}
</script>

<style>
body{
  margin: 0 !important;
}
::-webkit-scrollbar {
  width: 0;
}
.home__main{
  height: 100vh;
}
.home__sites{
  height:250vh;
}
.home__footer{
  height: 100vh;
}
.home__mail{
  height: 100vh;
}

.home__people{
  height: 100vh;
}
</style>
