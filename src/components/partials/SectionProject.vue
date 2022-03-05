<template>
  <section id="projects" class="py-5">
      <div class="container">
          <div class="row">
              <div class="col">
                  <img src="../../assets/img/men-data.png">
              </div>
              <div class="col">
                  <div class="text-white">start your project</div>
                  <div class="text-white">grow your business</div>
                  <div class="text-white">with our strategy</div>
                  <div class="ms_text">When, while the lovely valley teems with vapour around meand the meridian sun strikes the upper surface of the impenetrable follage of my trees, and but a few stray gleams steal into the inner sanctuary</div>
                  <div class="text-center">
                      <ButtonRed message="Try It Now"/>
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
        width: 75%;
        object-fit: contain;
    }
    .ms_text {
        color: $textP;
    }
}
</style>