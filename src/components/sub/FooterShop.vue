<template>
  <section>
    <div class="cards">
      <div class="card" v-for="card in cards" :key="card.text">

        <img :src="'../../assets/img/' + card.image" :alt="card.text">

        <h3>{{ card.text }}</h3>

      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'FooterShop',
  data(){
    return{
      cards:[
        {
          "text": "Digital Comics",
          "image":"buy-comics-digital-comics.png"
        },
        {
          "text": "DC Merchandise",
          "image": "buy-comics-merchandise.png"
        },
        {
          "text": "Subscriptions",
          "image": "buy-comics-subscriptions.png"
        },
        {
          "text": "Comic Shop Locator",
          "image": "buy-comics-shop-locator.png"
        },
        {
          "text": "DC Power Visa",
          "image": "buy-comics-dc-power-visa.svg"
        },
        
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

  section{
    background-color: #0282f9;
    color: white;
    padding: 50px 0;
  }
    
</style>
