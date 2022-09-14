<template>
  <div id="app">
    <!-- <ceshi-vue></ceshi-vue> -->
    <home-header></home-header>
  </div>
</template>

<script>
// import CeshiVue from "./component/Ceshi.vue";
import HomeHeader from "./pages/home/Home.vue";
export default {
  name: "App",
  components: {
    // CeshiVue,
    HomeHeader,
  },
};
</script>

<style lang="less">
* {
  touch-action: pan-y;
}
</style>
