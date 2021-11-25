<template>
    <div class="comic">

        <div class="img-container">
            <img :src="arguments.img" :alt="arguments.series">
        </div>

        <div class="text">{{ arguments.series }}</div>

        <!-- <div class="img-container">
            <img :src="img" :alt="series">
        </div>

        <div class="text">{{ series }}</div> -->

    </div>
</template>

<script>
export default {
  name: 'ContentComics',
  props:{
      arguments: Object
      /* img: String,
      series: String */
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    .comic{
        width: calc(100% / 6);

        .img-container{
            max-height: 200px;
            overflow: hidden;
            margin: 10px 0;
        }

        .text{
            padding-right: 30px;
        }
    }
    
</style>
