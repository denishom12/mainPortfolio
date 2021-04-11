<template>
<div class="peoples">
  <div class="onetwoPeople">
    <div class="people__one">
      <PeopleOne></PeopleOne>
    </div>
    <div class="people__two">
      <PeopleTwo></PeopleTwo>
    </div>

  </div>
</div>
</template>

<script>
import PeopleOne from "@/components/peopleOne";
import PeopleTwo from "@/components/peopleTwo";
export default {
  name: "peopleOneTwo",
  components: {PeopleOne, PeopleTwo}
}
</script>

<style>
.onetwoPeople{
  display: flex;
  flex-direction: row;
  justify-content: space-around;
  align-items: center;
  position: absolute;
  margin-top: 10%;
}
.people__one{
  width: 50%;
  position: relative;
}
.people__two{
  width: 50%;
  position: relative;
}

@media (max-width: 700px) {
  .onetwoPeople{
    flex-direction: column;
  }
  .people__one{
    margin-top: -15%;
  }
  .people__two{
    margin-top: 15%;
  }
  .onetwoPeople{
    margin-top: -20%;
  }
}
@media (max-width: 600px) {
  .people__one{
    margin-top: -15%;
  }
  .people__two{
    margin-top: 15%;
  }
  .onetwoPeople{
    margin-top: -20%;
  }
}

@media (max-width: 900px) {
  .onetwoPeople{
    flex-direction: column;
  }
  .people__one{
    margin-top: -15%;
  }
  .people__two{
    margin-top: 15%;
  }
  .onetwoPeople{
    margin-top: -20%;
  }
}

@media (max-width: 1300px) {
  .onetwoPeople{
    margin-top: 20%;
  }
}
@media (max-width: 1000px) {
  .onetwoPeople{
    margin-top: 20%;
  }
}
</style>