<template>
  <header>
    
    <div class="logo">
      <img src="../assets/img/dc-logo.png" alt="">
    </div>

    <nav>

      <ul>

        <li v-for="link, i in links" :key="i">
          <a :href="link.url" :class="link.active ? 'active' : ''">{{ link.text }}</a>
        </li>

      </ul>

    </nav>

  </header>
</template>

<script>
export default {
  name: 'Header',
  data(){
    return{
      links:[
        {
          "text": "Characters",
          "url": "#",
          "active": false
        },
        {
          "text": "Comics",
          "url": "#",
          "active": true
        },
        {
          "text": "Movies",
          "url": "#",
          "active": false
        },
        {
          "text": "TV",
          "url": "#",
          "active": false
        },
        {
          "text": "Games",
          "url": "#",
          "active": false
        },
        {
          "text": "Collectibles",
          "url": "#",
          "active": false
        },
        {
          "text": "Videos",
          "url": "#",
          "active": false
        },
        {
          "text": "Fans",
          "url": "#",
          "active": false
        },
        {
          "text": "News",
          "url": "#",
          "active": false
        },
        {
          "text": "Shop",
          "url": "#",
          "active": false
        },
        
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  header{
    width: 70%;
    margin: auto;
    height: 150px;
    display: flex;
    justify-content: space-between;
    align-items: center;

    .logo{
      width: 80px;

      img{
        max-width: 100%;
      }
    }

    nav{
    
      li{
        display: inline-block;

        a{
          margin: 0 20px;
          text-decoration: none;
          color: #1c1c1c;
          padding-bottom: 60px;

          &.active{
            color: #0282f9;
            border-bottom: solid 5px #0282f9;
          }

          &:hover{
            border-bottom: solid 5px #0282f978;
          }
        }
      }
    }
  }
</style>
