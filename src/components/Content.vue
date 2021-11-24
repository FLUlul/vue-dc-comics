<template>
  <section>
      <div>
            <h1>Content goes here</h1>
      </div>
  </section>
</template>

<script>
export default {
  name: 'Content',
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
          "active": false
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
    section{
        background-color: #1c1c1c;
        color: white;
        padding: 50px 0;
        div{
            width: 70%;
            margin: auto;
        }
    }
    
</style>
