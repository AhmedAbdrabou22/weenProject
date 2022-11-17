<template>
<div class='app'>
  <homePage />
</div>
  <!-- <router-view/> -->
</template>

<script>
import homePage from './components/homePage.vue'
export default {
  data() {
    return {

    }
  },
  components: {homePage}
}
</script>

<style>
::selection{
  background-color: black;
  color: white;;
}
body{
  background-color: #fafafa;
}
</style>
