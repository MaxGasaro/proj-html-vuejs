<template>
  <section id="pricelist" class="pt-5 mt-3">
      <InitSectionCenterWhite 
      sectionName="price list"
      title="pricing"
      titleBolder="our"
      paragraph="When, while the lovely valley teems with vapour around meand the meridian sun strikes the upper surface"  
      />
      <div class="container">
          <div class="row">
              <CardPriceList
              v-for="(item, indice) in items" :key="indice"
              :item="item"
              />
          </div>
      </div>
  </section>
</template>

<script>
import CardPriceList from './CardPriceList.vue'
import InitSectionCenterWhite from './InitSectionCenterWhite.vue'
export default {
    name: 'PriceList',
    components: {
        CardPriceList,
        InitSectionCenterWhite
    },
    data() {
        return {
            items: [
                {
                    title: 'Designing',
                    subtitle: 'PROCESS',
                    price: '40',
                    period: 'Per Month',
                    span1: 'Creative',
                    text1: 'Design Enabled',
                    span2: 'Vibrant',
                    text2: 'Color Usage',
                    span3: 'Eye',
                    text3: 'Catching Design',
                    span4: 'Extreme',
                    text4: 'Tipography',
                    span5: 'Exceptional',
                    text5: 'Design',
                    buttonContent: 'Order Now',
                    color: false,
                },
                {
                    title: 'Developing',
                    subtitle: 'PRODUCT',
                    price: '60',
                    period: 'Per Month',
                    span1: 'Creative',
                    text1: 'Design Enabled',
                    span2: 'Vibrant',
                    text2: 'Color Usage',
                    span3: 'Eye',
                    text3: 'Catching Design',
                    span4: 'Extreme',
                    text4: 'Tipography',
                    span5: 'Exceptional',
                    text5: 'Design',
                    buttonContent: 'Order Now',
                    color: true,
                },
                {
                    title: 'Supporting',
                    subtitle: 'CLIENTS',
                    price: '80',
                    period: 'Per Month',
                    span1: 'Creative',
                    text1: 'Design Enabled',
                    span2: 'Vibrant',
                    text2: 'Color Usage',
                    span3: 'Eye',
                    text3: 'Catching Design',
                    span4: 'Extreme',
                    text4: 'Tipography',
                    span5: 'Exceptional',
                    text5: 'Design',
                    buttonContent: 'Order Now',
                    color: false,
                },
            ]
        }
    }
}
</script>

<style scoped lang="scss">
@import '../../assets/style/variables.scss';
#pricelist {
    background-color: $backgroundPrimary;
    margin-bottom: 300px;
}
</style>