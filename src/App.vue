<script>
  import AppHeader from './components/AppHeader.vue';
  import AppMain from './components/AppMain.vue';

  export default {
    name:'App',
    components: {
      AppHeader,
      AppMain,
    },//components
  };//export
</script>

<template>
  <h1>Hello World!</h1>
  <AppHeader/>
</template>

<style  lang="scss">
	@import "./style/main";

</style>