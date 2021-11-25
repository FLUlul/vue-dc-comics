<template>
  <section id="footer-socials">
    
    <div class="container">

      <div class="btn">
        <a href="#">SIGN-UP NOW!</a>
      </div>

      <div class="socials">

        <h3>FOLLOW US</h3>

        <div class="logo-socials">

          <!-- <img :src="require(`../../assets/img/${social.logo}`)" alt=""> -->
          <img :src="require(`../../assets/img/footer-facebook.png`)" alt="" v-for="social, i in socials" :key="i">
          <!-- <p>{{ social.logo }}</p> -->
    
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
          "url": "#"
        },
        {
          "logo": "footer-twitter.png",
          "url": "#"
        },
        {
          "logo": "footer-youtube.png",
          "url": "#"
        },
        {
          "logo": "footer-periscope.png",
          "url": "#"
        },
        {
          "text": "footer-pintrest.png",
          "url": "#"
        }
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  #footer-socials{
    background-color: #303030;
    padding: 40px 0;

    .container{
      width: 70%;
      margin: auto;
      display: flex;
      justify-content: space-between;
      align-items: center;

      .btn{
        a{
          padding: 15px;
          border: solid #0282f9 3px;
          text-decoration: none;
          color: white;

        }
      }

      .socials{
        display: flex;
        align-items: center;
        
        
        h3{
          color: #0282f9;
          margin-right: 10px;
        }

        .logo-socials{
          display: flex;

          img{
            padding: 0 10px;
          }

        }
      }
    }
  }
    
</style>
