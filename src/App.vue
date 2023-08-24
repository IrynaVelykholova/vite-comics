<script>
  import TheHeader from "./components/TheHeader.vue";
  import dcComicsArray from "./dcComics.js";
  import comicsCards from "./components/comicsCards.vue";
  import TheFooter from "./components/TheFooter.vue";


  export default {
    components:{
      TheHeader,
      comicsCards,
      TheFooter,
    },
    data() {
      return {
        dcComicsArray,
      };
  },
}
    
</script>

<template> 
  <TheHeader></TheHeader>

  <main> 
    <div class=" black-main">
      <img class="img-jumbo" src="./assets/img/jumbotron.jpg" alt="">

      <div class="text-center position-relative">
        <button class="position-absolute button-blue button-absolute">CURRENT SERIES</button> 

        <div class="row row-cols-6 gy-3 my-5 card-container">

          <!-- ciclo for per le card -->
          <div class="card bg-black" 
            v-for="card in dcComicsArray">
            
            <comicsCards
              :imgSrc="card.thumb"
              :series="card.series" 
              :type="card.type"
              :price="card.price"
            >
            </comicsCards>
          </div>

          <button class="button-blue button-load">LOAD MORE</button>
        </div>
      </div>
    </div>
  </main>


</template>

<style lang="scss" scoped>
@use "./styles/partials/variables" as *;

.black-main {
  background-color: black;
  .img-jumbo {
      height: 450px;
      width: 100%;
      object-position: top;
      object-fit: cover;
    }
  .button-absolute {
    top: -12%;
    left: 15%;
  }
  .card-container {
      max-width: 1280px;
      margin: auto;
    }
  .button-blue {
    background-color: $color-primary;
    color: white;
    padding: 1rem 2rem;
    border: none;
  }
  .button-load {
    margin: auto;
  }
}
</style>