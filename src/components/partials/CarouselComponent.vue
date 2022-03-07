<template>
  
    <VueSlickCarousel v-bind="settings">
      <!--<div class="col-3">
        <img :src="require(`../../assets/img/${item.url}`)">
        <div class="d-flex justify-content-between">
         <p>{{item.textLeft}}</p>
         <p>{{item.textRight}}</p>
        </div>
      </div>-->
      <div class="col-3">
        <img :src="require(`../../assets/img/${items[0].url}`)">
        <div class="d-flex justify-content-between">
         <p>{{items[0].textLeft}}</p>
         <p>{{items[0].textRight}}</p>
        </div>
      </div>
      <div class="col-3">
        <img :src="require(`../../assets/img/${items[1].url}`)">
        <div class="d-flex justify-content-between">
         <p>{{items[1].textLeft}}</p>
         <p>{{items[1].textRight}}</p>
        </div>
      </div>
      <div class="col-3">
        <img :src="require(`../../assets/img/${items[2].url}`)">
        <div class="d-flex justify-content-between">
         <p>{{items[2].textLeft}}</p>
         <p>{{items[2].textRight}}</p>
        </div>
      </div>
      <div class="col-3">
        <img :src="require(`../../assets/img/${items[3].url}`)">
        <div class="d-flex justify-content-between">
         <p>{{items[3].textLeft}}</p>
         <p>{{items[3].textRight}}</p>
        </div>
      </div>
      <div class="col-3">
        <img :src="require(`../../assets/img/${items[4].url}`)">
        <div class="d-flex justify-content-between">
         <p>{{items[4].textLeft}}</p>
         <p>{{items[4].textRight}}</p>
        </div>
      </div>
    </VueSlickCarousel>
  
</template>

<script>
  import VueSlickCarousel from 'vue-slick-carousel'
  // optional style for arrows & dots
  import 'vue-slick-carousel/dist/vue-slick-carousel-theme.css'

  export default {
    name: 'CarouselComponent',
    props: {
        'items': Array
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
    components: { VueSlickCarousel },
  }
</script>

<style scoped lang="scss">
img {
    object-fit: contain;
    width: 100%;
    height: 100px;
}
</style>