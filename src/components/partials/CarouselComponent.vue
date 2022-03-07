<template>
  <div class="col-3">
    
      <!--<div class="col-3">
        <img :src="require(`../../assets/img/${item.url}`)">
        <div class="d-flex justify-content-between">
         <p>{{item.textLeft}}</p>
         <p>{{item.textRight}}</p>
        </div>
      </div>-->
        <img :src="require(`../../assets/img/${item.url}`)">
        <div class="d-flex pt-3 justify-content-between">
         <p class="fw-bold">{{item.textLeft}}</p>
         <p class="fw-lighter">{{item.textRight}}</p>
        </div>

  </div>
</template>

<script>
  //import VueSlickCarousel from 'vue-slick-carousel'
  // optional style for arrows & dots
  //import 'vue-slick-carousel/dist/vue-slick-carousel-theme.css'

  export default {
    name: 'CarouselComponent',
    props: {
        'item': Object
    },
    data() {
        return {
            settings: {
                "centerMode": true,
                "centerPadding": "20px",
                "focusOnSelect": true,
                "infinite": true,
                "slidesToShow": 3,
                "speed": 500,
                'arrows': true,
                'dots': true
            }
        }
    },
    //components: { VueSlickCarousel },
  }
</script>

<style scoped lang="scss">
img {
    object-fit: cover;
    width: 100%;
    height: 300px;
    border-radius: 30px;
}
</style>