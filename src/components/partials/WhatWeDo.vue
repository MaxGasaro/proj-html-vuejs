<template>
  <section id="what_we_do">
      <InitSectionCenter sectionName="our services" title="we do" titleBolder="what" paragraph="When, while the lovely valley teems with vapour around meand the"/>
      <div class="container">
          <div class="row pb-5">
              <CardWWD 
              v-for="(card, index) in cards" :key="index"
              :card="card"
              />
          </div>
      </div>
      <div class="d-flex justify-content-center py-5">
        <ButtonRed message="View All Services"/>
      </div>
  </section>
</template>

<script>
import InitSectionCenter from './InitSectionCenter.vue'
import CardWWD from './CardWWD.vue'
import ButtonRed from './ButtonRed.vue'
export default {
    name: 'WhatWeDo',
    components: {
        InitSectionCenter,
        CardWWD,
        ButtonRed
    },
    data() {
        return {
            cards: [
                {
                    img:'Group-247.png',
                    title: 'Data Analyst',
                    paragraph: 'When, while the lovely valley teems with vapour around meand the meridian sun strikes the upper'
                },
                {
                    img:'Group-538.png',
                    title: 'SEO Optimization',
                    paragraph: 'When, while the lovely valley teems with vapour around meand the meridian sun strikes the upper'
                },
                {
                    img:'Group-566.png',
                    title: 'Security Data',
                    paragraph: 'When, while the lovely valley teems with vapour around meand the meridian sun strikes the upper'
                },
                {
                    img:'Group-567.png',
                    title: 'Branding Strategy',
                    paragraph: 'When, while the lovely valley teems with vapour around meand the meridian sun strikes the upper'
                },
            ]
        }
    }
}
</script>

<style scoped lang="scss">

</style>