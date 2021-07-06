<template>
  <div id="app">
    <Header/>
    <Main/>
    <MenuSection/>
  </div>
</template>

<script>
import Header from '@/components/Header.vue';
import Main from '@/components/Main.vue';
import MenuSection from '@/components/MenuSection.vue';

export default {
  name: 'App',
  components: {
    Header,
    Main,
    MenuSection
  }
}
</script>

<style lang="scss">
@import 'style/commons.scss';



</style>
