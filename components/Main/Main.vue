<template>
  <div class="container">
    <Banner/>
    <Instruction/>
    <AppropriateExercise/>
    <Posts/>
    <SendData/>
  </div>
</template>

<style>
.container {
  width: 1240px;
  margin: 0 auto;
}

@media (max-width: 1320px) {
  .container {
    width: 980px;
  }
}

@media (max-width: 1050px) {
  .container {
    width: 768px;
  }
}

@media (max-width: 820px){
  .container {
    width: 480px;
  }
}
</style>

<script setup>
import Banner from "@/components/Main/MainComponents/Banner.vue";
import Instruction from "@/components/Main/MainComponents/Instruction.vue";
import AppropriateExercise from "@/components/Main/MainComponents/AppropriateExercise.vue";
import Posts from "@/components/Main/MainComponents/Posts.vue";
import SendData from "@/components/Main/MainComponents/SendData.vue";
</script>
