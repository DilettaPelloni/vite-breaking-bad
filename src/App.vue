<script>
    import AppHeader from './components/AppHeader.vue';
    import AppMain from './components/AppMain.vue';
    import axios from 'axios';
    import {store} from './store';

    export default {
        name:'App',
            components: {
            AppHeader,
            AppMain,
        },//components
        data() {
            return {
                store,
            };//return
        },//data
        created() {
            axios.get('https://db.ygoprodeck.com/api/v7/cardinfo.php').then((response) => {
                this.store.cards = response.data.data.slice(0,20);
                this.store.loaded = true;
            });
        },//created
    };//export
</script>

<template>
    <AppHeader/>
    <AppMain/>
</template>

<style  lang="scss">
@import "./style/main.scss";

</style>