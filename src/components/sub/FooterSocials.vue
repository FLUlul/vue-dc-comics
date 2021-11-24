<template>
  <section id="footer-socials">
    
    <div class="container">

      <div class="btn">
        <a href="#">SIGN-UP NOW!</a>
      </div>

      <div class="socials">

        <h3>FOLLOW US</h3>

        <div class="logo-socials" v-for="social, i in socials" :key="i">

          <img :src="require(`../../assets/img/${social.logo}`)" :alt="social.logo">
    
        </div>

      </div>

    </div>

  </section>
</template>

<script>
export default {
  name: 'FooterSocials',
  data(){
    return{
      socials:[
        {
          "logo": "footer-facebook.png",
          "url": "#",
        },
        {
          "logo": "footer-twitter.png",
          "url": "#",
        },
        {
          "logo": "footer-youtube.png",
          "url": "#",
        },
        {
          "logo": "footer-periscope.png",
          "url": "#",
        },
        {
          "text": "footer-pintrest.png",
          "url": "#",
        },
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  section{
    background-color: #303030;

    .container{
      width: 70%;
      margin: auto;
    }
  }
    
</style>
