<template>
  <section id="projects" class="p-5">
      <div class="container">
          <div class="row">
              <div class="col">
                  <img src="../../assets/img/men-data.png">
              </div>
              <div class="col d-flex flex-column justify-content-center">
                  <div class="text-white text-capitalize">start your project</div>
                  <div class="text-white fs-1 text-capitalize fw-bolder pt-3">grow your business</div>
                  <div class="text-white fs-1 text-capitalize pb-4">with our strategy</div>
                  <div class="ms_text pb-4">When, while the lovely valley teems with vapour around meand the meridian sun strikes the upper surface of the impenetrable follage of my trees, and but a few stray gleams steal into the inner sanctuary</div>
                  <div class="d-flex">
                      <ButtonRed class="me-3" message="Try It Now"/>
                      <ButtonBlue message="Explore More"/>
                  </div>
              </div>
          </div>
      </div>
  </section>
</template>

<script>
import ButtonBlue from './ButtonBlue.vue'
import ButtonRed from './ButtonRed.vue'
export default {
    name: 'SectionProject',
    components: {
        ButtonBlue,
        ButtonRed
    }
}
</script>

<style scoped lang="scss">
@import '../../assets/style/variables.scss';
#projects {
    background-color: $backgroundPrimary;
    img {
        width: 60%;
        object-fit: contain;
    }
    .ms_text {
        color: $textP;
        font-size: 12px;
    }
}
</style>