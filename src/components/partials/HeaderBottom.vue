<template>
  <div class="container">
      <div class="row">
          <div class="col">
              <h1>business planning</h1>
              <h1>digital technology</h1>
              <h1>modern solution!</h1>
              <p>When, while the lovely valley teems with vapour around meand the meridian sun strikes the upper surface.</p>
              <ButtonRed message="Try It Now"/>
              <ButtonBlue message="Explore More"/>
          </div>
          <div class="col">
              <img src="../../assets/img/header.png" alt="foto header">
          </div>
      </div>
  </div>
</template>

<script>
import ButtonBlue from '../partials/ButtonBlue.vue'
import ButtonRed from '../partials/ButtonRed.vue'
export default {
    name: 'HeaderBottom',
    components: {
        ButtonBlue,
        ButtonRed
    }
}
</script>

<style scoped lang="scss">
@import '../../assets/style/variables.scss';
h1 {
    color: $primaryText;
    text-transform: capitalize;
}
p {
    color: $textP;
}
img {
    max-width: 75%;
    object-fit: contain;
}
</style>