<template>
  <section id="footer-nav">

    <div class="container">

      <nav class="nav-container">

        <div class="left-block">

          <h3>{{ lists[0].title }}</h3>

          <ul>
            <li v-for="content, j in lists[0].contents" :key="j">
              {{ content.text }}
            </li>
          </ul>

          <h3 id="shop">{{ lists[1].title }}</h3>

          <ul>
            <li v-for="content, j in lists[1].contents" :key="j">
              {{ content.text }}
            </li>
          </ul>

        </div>

        <div class="mid-block">

          <h3>{{ lists[2].title }}</h3>

          <ul>
            <li v-for="content, j in lists[2].contents" :key="j">
              {{ content.text }}
            </li>
          </ul>

        </div>

        <div class="right-block">

          <h3>{{ lists[3].title }}</h3>

          <ul>
            <li v-for="content, j in lists[3].contents" :key="j">
              {{ content.text }}
            </li>
          </ul>

        </div>

      </nav>

      <div class="image">
        <img src="../../assets/img/dc-logo-bg.png" alt="">
      </div>

    </div>

  </section>
</template>

<script>
export default {
  name: 'FooterNav',
  data(){
    return{
      lists:[
        {
          "title": "DC Comics",
          "contents":[
            {
              "text": "Characters"
            },
            {
              "text": "Comics"
            },
            {
              "text": "Movies"
            },
            {
              "text": "TV"
            },
            {
              "text": "Games"
            },
            {
              "text": "Videos"
            },
            {
              "text": "News"
            }, 
          ]
        },
        {
          "title": "Shop",
          "contents":[
            {
              "text": "Shop DC"
            },
            {
              "text": "Shop DC Collectibles"
            },            
          ]
        },
        {
          "title": "DC",
          "contents":[
            {
              "text": "Term Of Use"
            },
            {
              "text": "Privacy policy(New)"
            },
            {
              "text": "Ad Choices"
            },
            {
              "text": "Advertising"
            },
            {
              "text": "Jobs"
            },
            {
              "text": "Subscriptions"
            },
            {
              "text": "Talent Workshops"
            },
            {
              "text": "CPSC Certificates"
            },
            {
              "text": "Ratings"
            },
            {
              "text": "Shop Help"
            },
            {
              "text": "Contact Us"
            },
          ]
        },
        {
          "title": "Sites",
          "contents":[
            {
              "text": "DC"
            },
            {
              "text": "MAD Magazine"
            },
            {
              "text": "DC Kids"
            },
            {
              "text": "DC Universe"
            },
            {
              "text": "DC Power Visa"
            },            
          ]
        },
        
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

    #footer-nav{
      background-image: url("../../assets/img/footer-bg.jpg");
      background-position: center;
      background-size: cover;

      .container{
        display: flex;
        width: 70%;
        margin: auto;
        overflow: hidden;
        padding: 50px 0;

        .nav-container{
          display: flex;
          width: 50%;

          h3{
            color: white;
            margin-right:20px;
          }

          ul{
            margin-right:20px;
            margin-top: 10px;
            li{
              color: #838383;
              list-style: none;
              margin: 5px 0;
            }
          }


          #shop{
            margin-top: 20px;
          }
        }
        
        .image {
          position: relative;
          display: flex;
          align-items: center;
          justify-content: flex-end;
          width: 50%;

          img{
            position: absolute; 

          }
        }
      }
      
    }

</style>
