<script>
    import {store} from '../store';
    export default {
        name:'MainCounter',
        data() {
            return {
                store,
            };//return
        },//data
    };//export
</script>

<template>
    <div class="row bg-dark text-light fw-bold ">
            <p class="m-0 py-2 ">Found {{store.cards.length}} cards</p>
    </div><!-- CHIUSURA ROW DI TESTA -->
</template>

<style  lang="scss" scoped>
</style>