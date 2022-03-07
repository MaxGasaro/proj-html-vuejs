<template>
<div id="header_bottom">
  <div class="container h-100">
      <div class="row align-items-center h-100">
          <div class="col">
              <h1 class="fw-bolder">business planning</h1>
              <h1 class="fw-lighter">digital technology</h1>
              <h1 class="fw-bolder">modern solution!</h1>
              <p class="py-3">When, while the lovely valley teems with vapour around <br> meand the meridian sun strikes the upper surface.</p>
              <div class="d-flex">
                <ButtonRed class="me-3" message="Try It Now"/>
                <ButtonBlue message="Explore More"/>
              </div>
          </div>
          <div class="col d-flex justify-content-center">
              <img src="../../assets/img/header.png" alt="foto header">
          </div>
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
#header_bottom {
    height: calc(100% - 50px);
    h1 {
        color: $primaryText;
        text-transform: capitalize;
    }
    p {
        color: $textP;
        font-size: 12px;
    }
    img {
        max-width: 75%;
        object-fit: contain;
    }
}
</style>