<template lang="pug">
  section.container
    cursorPointer
    h1 toppage
</template>

<script>
import cursorPointer from '@/components/cursorPointer'

export default {
  components: {
    cursorPointer
  },
  mounted(){
  }
}
</script>

<style lang="scss" scoped>
h1{
  color: red;
}
</style>
