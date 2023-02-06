<script>
  export default {
    name:'AppMain',
  }
</script>

<template>
    <main class="py-4">
      <div class="container">
        <section class="mb-4">
          <select name="filter" >
            <option value="Alien" selected>
              Alien
            </option>
          </select>
        </section><!-- CHIUSURA SEZIONE SELECT -->
        <section class="p-5 bg-light">
          <div class="row py-2 bg-dark text-light fw-bold">
            <p class="m-0">Found x cards</p>
          </div><!-- CHIUSURA ROW DI TESTA -->
          <div class="row row-cols-5">
            <div class="col my-card p-0 text-center">
              <img class="img-fluid" src="https://i.ebayimg.com/images/g/Y-kAAOSw2ppg7dl3/s-l500.jpg" alt="prova">
              <p class="my-3 text-light fw-bold">EXODIA</p>
              <p class="m-0">alieno</p>
            </div>
          </div>
        </section><!-- CHIUSURA SEZIONE CARD BOX -->
      </div><!-- CHIUSURA CONTAINER -->
    </main>
</template>

<style  lang="scss" scoped>
main {
  background-color: $main-orange;
}

.my-card {
  background-color: $main-orange;
}
</style>