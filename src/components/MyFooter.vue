<template>
  <footer>
      <FooterTop :quickLinks="quickLinks" :resources="resources"/>
      <FooterBottom/>
  </footer>
</template>

<script>
import FooterTop from './partials/FooterTop.vue'
import FooterBottom from './partials/FooterBottom.vue'
export default {
    name: 'MyFooter',
    props: {
      'quickLinks': Array,
      'resources': Array
    },
    components: {
      FooterTop,
      FooterBottom
    }

}
</script>

<style scoped lang="scss">
@import '../assets/style/variables.scss';
footer {
  background-color: $backgroundPrimary;
  color: $primaryText;
}

</style>