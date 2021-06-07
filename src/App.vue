<template>
  <div id="app">
      <Header />
      <Main />
      <Footer />
  </div>
</template>

<script>
import Header from '@/components/Header.vue';
import Main from '@/components/Main.vue';
import Footer from '@/components/Footer.vue';

export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer
  }
}
</script>

<style lang="scss">
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

#app {
  height: 100vh;
}

.container {
  width: 70%;
  margin: 0 auto;
}

.bar {
  height: 150px;
}

.float {
  float: left;
}
.clearfix::after {
  content: '';
  display: table;
  clear: both;
}
</style>
