<script setup>
  import Title from './components/Title.vue';
  import Portportio from './components/Portfolio.vue';
  import About from './components/About.vue';
  import Navbar from './components/Navbar.vue';
  import data from './assets/portfolio';

</script>

<template>
  <Navbar/>
  <router-view :data="data" />
</template>

<style scoped lang="scss">

</style>