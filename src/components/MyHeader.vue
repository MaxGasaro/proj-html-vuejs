<template>
  <header>
    <HeaderTop :itemsNav="itemsNav"/>
    <HeaderBottom/>
  </header>
</template>

<script>
import HeaderTop from './partials/HeaderTop.vue'
import HeaderBottom from './partials/HeaderBottom.vue'
export default {
    name: 'MyHeader',
    props: {
      'itemsNav': Array
    },
    components: {
      HeaderTop,
      HeaderBottom
    }
}
</script>

<style scoped lang="scss">
@import '../assets/style/variables.scss';
header {
  height: 60vh;
  background-color: $backgroundPrimary;
  padding: 2rem;
}

</style>