<template>

  <article>
    <section class="gallery">
      <div class="card-wrapper">
        <div class="card">
          <div class="card-overlay" v-for="item in sortedStockedProducts" :key="item.id">
            <h1 class="card-overlay-heading">{{item.titel}}</h1>
            <p class="card-overlay-paragraph">{{item.price}}</p>
            <button class="card-overlay-button"><router-link :to="'/detail/' + item.id">Koop nu</router-link></button>
            <router-view></router-view>
          </div>
          <!--<img :src="'@/assets/' + item.afbeelding" alt="guitar1" class="card-image">-->
          <!--<img :src="require(`@/assets/${item.afbeelding}`)" alt="guitar1" class="card-image">-->
          <img :src="'@/assets/${item.afbeelding}'" :alt="item.titel" class="card-image">
        </div>
      </div>
    </section>

    <!--<section class="gallery">
      <div class="card-wrapper">
        <div class="card" v-for="item in sortedStockedProducts" :key="item.id">
          <div class="card-overlay">
            <h1 class="card-overlay-heading">{{ item.titel }}</h1>
            <p class="card-overlay-paragraph">{{ item.price }}</p>
            <button class="card-overlay-button">
              <router-link :to="'/detail/' + item.id">Koop nu</router-link>
            </button>
            <router-view></router-view>
          </div>
          <img :src="'@/assets/' + item.afbeelding" :alt="item.titel" class="card-image">
        </div>
      </div>
    </section>-->


    <section class="gallery">
      <div class="card-wrapper">
        <div class="card">
          <div class="card-overlay" v-for="item in sortedStockedProducts" :key="item.id">
            <h1 class="card-overlay-heading">{{item.titel}}</h1>
            <p class="card-overlay-paragraph">{{item.price}}</p>
            <button class="card-overlay-button"><router-link :to="'/detail/' + item.id">Koop nu</router-link></button>
            <router-view></router-view>
          </div>
          <!--<img :src="'@/assets/' + item.afbeelding" alt="guitar1" class="card-image">-->
          <!--<img :src="require(`@/assets/${item.afbeelding}`)" alt="guitar1" class="card-image">-->
          <img :src="'@/assets/${item.afbeelding}'" :alt="item.titel" class="card-image">
        </div>
      </div>
    </section>



    <section class="gallery">
      <div class="card-wrapper">
        <div class="card">
          <div class="card-overlay" v-for="item in sortedStockedProducts" :key="item.id">
            <h1 class="card-overlay-heading">{{item.titel}}</h1>
            <p class="card-overlay-paragraph">{{item.price}}</p>
            <button class="card-overlay-button"><router-link :to="'/detail/' + item.id">Koop nu</router-link></button>
            <router-view></router-view>
          </div>
          <!--<img :src="'@/assets/' + item.afbeelding" alt="guitar1" class="card-image">-->
          <!--<img :src="require(`@/assets/${item.afbeelding}`)" alt="guitar1" class="card-image">-->
          <img :src="'@/assets/${item.afbeelding}'" :alt="item.titel" class="card-image">
        </div>
      </div>
    </section>



    <section class="gallery">
      <div class="card-wrapper">
        <div class="card">
          <div class="card-overlay" v-for="item in sortedStockedProducts" :key="item.id">
            <h1 class="card-overlay-heading">{{item.titel}}</h1>
            <p class="card-overlay-paragraph">{{item.price}}</p>
            <button class="card-overlay-button"><router-link :to="'/detail/' + item.id">Koop nu</router-link></button>
            <router-view></router-view>
          </div>
          <!--<img :src="'@/assets/' + item.afbeelding" alt="guitar1" class="card-image">-->
          <!--<img :src="require(`@/assets/${item.afbeelding}`)" alt="guitar1" class="card-image">-->
          <img :src="'@/assets/${item.afbeelding}'" :alt="item.titel" class="card-image">
        </div>
      </div>
    </section>


  </article>


  <!--<article>
    <section class="gallery">
      <div class="card-wrapper">
        <div class="card">
          <div class="card-overlay" v-for="product in producten" :key="product.id">
            <h1 class="card-overlay-heading">{{product.titel}}</h1>
            <p class="card-overlay-paragraph">{{product.price}}</p>
            <button class="card-overlay-button"><router-link to="/detail">Koop nu</router-link></button>
            <router-view></router-view>
          </div>
          <img :src="require('@/assets/' + product.afbeelding)" alt="guitar1" class="card-image">
        </div>
      </div>
    </section>
  </article>-->


  <!--<article>
    <section class="gallery">
      <div class="card-wrapper">
        <div class="card">
          <div class="card-overlay">
            <h1 class="card-overlay-heading">ESP era5S11</h1>
            <p class="card-overlay-paragraph">Prijs: €15 000</p>
            <button class="card-overlay-button">Meer info</button>
          </div>
          <img src="@/assets/guitar-T.png" alt="guitar6" class="card-image">
        </div>
      </div>
    </section>
    <section class="gallery">
      <div class="card-wrapper">
        <div class="card">
          <div class="card-overlay">
            <h1 class="card-overlay-heading">Gibson E-455</h1>
            <p class="card-overlay-paragraph">Prijs: €11 000</p>
            <button class="card-overlay-button">Meer info</button>
          </div>
          <img src="@/assets/guitar-T-2.png" alt="guitar7" class="card-image">
        </div>
      </div>
    </section>
    <section class="gallery">
      <div class="card-wrapper">
        <div class="card">
          <div class="card-overlay">
            <h1 class="card-overlay-heading">Fender stratocaster Er-5</h1>
            <p class="card-overlay-paragraph">Prijs: €20 000</p>
            <button class="card-overlay-button">Meer info</button>
          </div>
          <img src="@/guitar-T-3.png" alt=" guitar8" class="card-image">
        </div>
      </div>
    </section>
    <section class="gallery">
      <div class="card-wrapper">
        <div class="card">
          <div class="card-overlay">
            <h1 class="card-overlay-heading">Fender Stratocaster Er-10</h1>
            <p class="card-overlay-paragraph">Prijs: €20 000</p>
            <button class="card-overlay-button">Meer info</button>
          </div>
          <img src="@/assets/guitar-T-4.png" alt="guitar9" class="card-image">
        </div>
      </div>
    </section>
  </article>-->
</template>

<script>

import producten from '@/json/producten.json';

export default {
  name: "PopularProductsComponent",

  /*methods: {
    getAfbeelding(item){
      if (item && item.afbeelding) {
        return `@/assets/${item.afbeelding}`;
      }
      // Als afbeelding niet gedefinieerd is, retourneer een standaardbeeld of een lege string
      return "@/assets/default-image.jpg";
    }
  },*/

  /*props: {
    products: Array
  },

  computed: {
    producten(){
      return this.products.slice(0,4);
    }
  },*/

  data(){
    return {
      data: producten
    }
  },
  
  computed: {
    sortedStockedProducts() {
      // Sorteer producten op basis van stock (aflopend)
      //const sorted = this.data.sort((a, b) => b.stock - a.stock);
      // Selecteer de eerste 3 tot 5 producten
      //return sorted.slice(0, 1);
      const sorted = this.data.sort((a, b) => b.stock - a.stock)
      return sorted.slice(0, 4);
    }
  }
};
</script>

<style scoped>

</style>