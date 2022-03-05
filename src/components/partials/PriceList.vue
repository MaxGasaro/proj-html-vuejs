<template>
  <section id="pricelist" class="pt-5 mt-3">
      <InitSectionCenter 
      sectionName="price list"
      title="pricing"
      titleBolder="our"
      paragraph="When, while the lovely valley teems with vapour around meand the meridian sun strikes the upper"  
      />
      <div class="container">
          <div class="row">
              <CardPriceList
              v-for="(item, index) in items" :key="index"
              :item="item"
              />
          </div>
      </div>
  </section>
</template>

<script>
import CardPriceList from './CardPriceList.vue'
import InitSectionCenter from './InitSectionCenter.vue'
export default {
    name: 'PriceList',
    components: {
        CardPriceList,
        InitSectionCenter
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
    margin-bottom: 400px;
}
</style>