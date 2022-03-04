<template>
  <section id="what_we_do">
      <InitSectionCenter sectionName="our services" title="we do" titleBolder="what" paragraph="When, while the lovely valley teems with vapour around meand the"/>
      <div class="container">
          <div class="row">
              <CardWWD textUp="Data Analyst"/>
              <CardWWD textUp="SEO Optimization"/>
              <CardWWD textUp="Security Data"/>
              <CardWWD textUp="Branding Strategy"/>
          </div>
      </div>
  </section>
</template>

<script>
import InitSectionCenter from './InitSectionCenter.vue'
import CardWWD from './CardWWD.vue'
export default {
    name: 'WhatWeDo',
    components: {
        InitSectionCenter,
        CardWWD
    }
}
</script>

<style scoped lang="scss">

</style>