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
    <AppHeader/>
    <AppMain/>
</template>

<style  lang="scss">
@import "./style/main.scss";

</style>