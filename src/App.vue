<template>
  <div id="app">
    <Header/>
    <Main/>
    <MenuSection/>
    <Footer/>
  </div>
</template>

<script>
import Header from '@/components/Header.vue';
import Main from '@/components/Main.vue';
import MenuSection from '@/components/MenuSection.vue';
import Footer from '@/components/Footer.vue';

export default {
  name: 'App',
  components: {
    Header,
    Main,
    MenuSection,
    Footer
  }
}
</script>

<style lang="scss">
@import 'style/commons.scss';



</style>
