<template>
<div class="site__panel">
  <img class="blop__image__sites" src="../assets/blop10.svg" alt="">
 <div class="site__contain">
   <div class="site__contain1">
     <div>
       <h1>Site for Google</h1>
       <p>Это одна из первых наших работ</p>
     </div>
     <div>
       <router-link to="/first"><FirstSite class="image__one"></FirstSite></router-link>
     </div>
   </div>

   <div class="site__contain2">
     <div>
       <h1>Site for Google</h1>
       <p>Это одна из первых наших работ</p>
     </div>
     <div>
       <router-link to="/first"><SecondSite class="image__one"></SecondSite></router-link>
     </div>
   </div>

   <div class="site__contain3">
     <div>
       <h1>Site for Google</h1>
       <p>Это одна из первых наших работ</p>
     </div>
     <div>
       <router-link to="/first"><ThirdSite class="image__one"></ThirdSite></router-link>
     </div>
   </div>

 </div>


</div>
</template>

<script>
import FirstSite from "@/components/firstSite";
import SecondSite from "@/components/secondSite";
import ThirdSite from "@/components/thirdSite";
export default {
name: "sitePanel",
  components: {ThirdSite, SecondSite, FirstSite}
}
</script>

<style>
.blop__image__sites{
  margin-top: -0.25%;
}
.image__one{
  transform: scale(0.3);
}
.site__panel{
  background-color: #f300b4;
  height: 330vh;
}


</style>