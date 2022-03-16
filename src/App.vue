<template>
  <Main msg="Welcome to Your Vue.js App"/>
</template>

<script>
import Main from './components/Main.vue'

export default {
  name: 'App',
  components: {
    Main
  }
}
</script>

<style lang="scss">
  @import url('https://fonts.googleapis.com/css2?family=Mulish:wght@200;300;500&display=swap');

  #app {
    margin: 0;
    padding: 0;
    font-family: 'Mulish', sans-serif;
    font-style: normal;
    font-weight: 200;
  }
</style>
