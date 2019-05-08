<template lang="pug">
  .container
    cursorPointer
    section
      lottie.first-view__wrap--image(
        :options="lottieOptions"
        v-on:animCreated="handleAnimation")
</template>

<script>
import * as animationData from "~/assets/json/my_logo.json";
import Lottie from "~/components/Lottie.vue";
import cursorPointer from '@/components/cursorPointer'

export default {
  components: {
    Lottie,
    cursorPointer
  },
  data(){
    return {
      lottieOptions: {
        animationData: animationData,
        loop: true,
      },
    }
  },
  mounted(){
  }
}
</script>

<style lang="scss" scoped>
section{
  height: 100vh;
  width: 100vw;
}
h1{
  color: red;
}
</style>
