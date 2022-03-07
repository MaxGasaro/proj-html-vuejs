<template>

  <section id="latest_works">
      <div class="container">
          <div class="row">
              <div class="ms_little_title_red col">
                  Portfolio
              </div>
          </div>
          <div class="row justify-content-between">
              <div class="col">
                  <span>latest</span> work
              </div>
              <div class="col text-end">
                  <i class="fa-solid fa-arrow-left-long"></i>
                  <i class="fa-solid fa-arrow-right-long"></i>
              </div>
          </div>
      </div>
      <div class="container-fluid">
          <div class="row flex-nowrap ms_overflow g-5">
              <CarouselComponent
              v-for="(item, index) in items" :key="index"
              :item="item"
              />
            </div>
          <div class="row justify-content-center">
              <div class="col d-flex justify-content-center">
                  <div 
                     v-for="n,index in 5" :key="index" class="active_check" :class="index=indice?'active':''">
                  </div>
              </div>
          </div>
      </div>
  </section>
</template>

<script>
import CarouselComponent from './CarouselComponent.vue'
export default {
    name: 'LatestWorks',
    components: {
        CarouselComponent
    },
    data() {
        return {
            items: [
                {
                    url: '8wa60okr-1-790x576.jpg',
                    textLeft: 'Basket of Flower on table',
                    textRight: 'Branding Strategy'
                },
                {
                    url: '84316050-0af0-49db-a53a-241d47ddad0e-2-790x576.jpg',
                    textLeft: 'Purinky Products',
                    textRight: 'Digital Experience'
                },
                {
                    url: 'a247b00b-3621-470f-b4b8-b3ac46f25907-1-790x576.jpg',
                    textLeft: 'Satisfy Poster',
                    textRight: 'Branding Strategy'
                },
                {
                    url: 'DRY-1-790x576.jpg',
                    textLeft: 'Mock Up',
                    textRight: 'Branding Strategy'
                },
                {
                    url: '84316050-0af0-49db-a53a-241d47ddad0e-2-790x576.jpg',
                    textLeft: 'Satisfy Poster',
                    textRight: 'Digital Experience'
                },
            ]
        }
    }
}
</script>

<style scoped lang="scss">
@import '../../assets/style/general.scss';
@import '../../assets/style/variables.scss';
#latest_works {
    // .ms_overflow {
    //     overflow-x: auto;
        // img {
        //     object-fit: contain;
        //     width: 100%;
        // }
    .active_check {
        width: 8px;
        height: 8px;
        border-radius: 50%;
        background-color: lightgray;
        margin: 8px 4px;
    }
    .active {
        background-color: red;
    }
}

</style>