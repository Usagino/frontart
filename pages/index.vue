<template lang="pug">
  .container
    cursorPointer
    
    section
      .first
        .first__wrap
          .first__wrap__logo
            lottie.first-view__wrap--image(
              :options="lottieOptions"
              v-on:animCreated="handleAnimation")
</template>

<script>
import * as animationData from "~/assets/json/my_logo.json";
import Lottie from "~/components/Lottie.vue";
import sideMenu from "~/components/sideMenu.vue";
import cursorPointer from '@/components/cursorPointer'

export default {
  components: {
    Lottie,
    cursorPointer,
    sideMenu
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
  .first{
    &__wrap{
      height: 100vh;
      width: 100vw;
      @include middle;
      &__logo{
        width: 40vw;
        height: auto;
      }
    }
  }
}

</style>
