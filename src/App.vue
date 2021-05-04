<template>
  <div id="app">
      <!--HEADER-->
      <Header />


      <!--MAIN-->
      <main>Main content here</main>

      <!--FOOTER-->
      <footer>Footer here</footer>
    
  </div>
</template>

<script>
import Header from '@/components/Header.vue';

export default {
  name: 'App',
  components: {
    Header
  }
}
</script>

<style lang="scss">

/* GENERAL */
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

body {
  font-family: 'Roboto Condensed', sans-serif;
}

a {
  color: #000;
}

</style>
