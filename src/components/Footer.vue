<template>
  <footer>
    <FooterShop/>
    <FooterNav/>
    <FooterSocials/>
  </footer>
</template>

<script>
import FooterShop from '@/components/sub/FooterShop.vue'
import FooterNav from '@/components/sub/FooterNav.vue'
import FooterSocials from '@/components/sub/FooterSocials.vue'

export default {
  name: 'Footer',
  components: {
    FooterShop,
    FooterNav,
    FooterSocials
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

</style>
