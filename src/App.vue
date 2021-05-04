<template>
  <div id="app">
      <!--HEADER-->
      <Header />


      <!--MAIN-->
      <Maincontent />
      <Marketing />

      <!--FOOTER-->
      <footer>Footer here</footer>
    
  </div>
</template>

<script>
import Header from '@/components/Header.vue';
import Maincontent from '@/components/Maincontent.vue';
import Marketing from '@/components/Marketing.vue';

export default {
  name: 'App',
  components: {
    Header,
    Maincontent,
    Marketing,
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
