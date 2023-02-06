<script>
import {store} from '../store';
    export default {
        name:'AppMain',
        data() {
            return {
                store,
            };//return
        },//data
    };//export
</script>

<template>
    <main class="py-4 bg-primary">
        <div class="container">
            <section class="mb-4">
                <select name="filter" >
                    <option value="Alien" selected>
                        Alien
                    </option>
                </select>
            </section><!-- CHIUSURA SEZIONE SELECT -->
            <section class="p-5 bg-light">
                <div class="row bg-dark text-light fw-bold ">
                        <p class="m-0 py-2 ">Found {{store.cards.length}} cards</p>
                </div><!-- CHIUSURA ROW DI TESTA -->
                <div class="row row-cols-5 justify-content-between g-3">
                    <div class="col text-center"
                        v-for="card in store.cards">
                        <div class="my-card h-100 bg-primary ">
                            <img class="img-fluid" :src="card.card_images[0].image_url_small" :alt="card.name">
                            <p class="my-3 text-light fw-bold">{{card.name}}</p>
                            <p class="m-0">{{card.type}}</p>
                        </div><!-- CHIUSURA CARD -->
                    </div><!-- CHIUSURA COL CARD -->
                </div><!-- CHIUSURA ROW CARDS -->
            </section><!-- CHIUSURA SEZIONE CARD BOX -->
        </div><!-- CHIUSURA CONTAINER -->
    </main>
</template>

<style  lang="scss" scoped>
</style>