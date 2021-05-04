<template>
  <div id="app">
      <!--HEADER-->
      <Header />


      <!--MAIN-->
      <Maincontent />
      <Marketing />

      <!--FOOTER-->
      <Footer />
    
  </div>
</template>

<script>
import Header from '@/components/Header.vue';
import Maincontent from '@/components/Maincontent.vue';
import Marketing from '@/components/Marketing.vue';
import Footer from '@/components/Footer.vue';

export default {
  name: 'App',
  components: {
    Header,
    Maincontent,
    Marketing,
    Footer,
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
