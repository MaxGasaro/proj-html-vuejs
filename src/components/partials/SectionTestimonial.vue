<template>
  <section id="testimonial">
      <InitSectionCenter
        sectionName="Testimonial"
        title="People Say"
        titleBolder="What"
        paragraph="When, while the lovely valley teems vapour around meand the meridian sun strikes the upper surface."
      />
      <div class="container">
        <div class="row row-cols-3">
          <CardTestimonial 
          v-for="(testimonial, index) in testimonials"
          :key="index"
          :testimonial="testimonial"
          />
        </div>
      </div>
      <div class="container py-5">
        <div class="row row-cols-5">
          <CardClients 
          v-for="(client, index) in clients"
          :key="index"
          :client="client"
          />
        </div>
      </div>
      <div class="container ms_section_offer">
        <div class="row align-items-center h-100">
          <div class="col d-flex flex-column">
            <div class="fs-4 fw-bolder">We Offer Awesome Services</div>
            <div class="">When, while lovely valley teems with vapour around meand meridian sun strikes the upper surface.</div>
          </div>
          <div class="col">
            <input type="text" placeholder="Enter Your Email Address">
          </div>
        </div>
      </div>
  </section>
</template>

<script>
import InitSectionCenter from './InitSectionCenter.vue'
import CardTestimonial from './CardTestimonial.vue'
import CardClients from './CardClients.vue'
export default {
    name: 'SectionTestimonial',
    components: {
        InitSectionCenter,
        CardTestimonial,
        CardClients
    },
    data() {
      return {
        testimonials: [
          {
            url: 'szabo-viktor-1266895-unsplash-1024x1024.png',
            vote: 3,
            text: 'When, while lovely valley teems with vapor around meand meridian sun strikes the upper impenetrable foliage of my trees, and but a thousand.',
            name: 'Michkel Anegl',
            position: 'Marketing Management'
          },
          {
            url: 'philipe-cavalcante-539505-unsplash-1024x1024.png',
            vote: 3,
            text: 'When, while lovely valley teems with vapor around meand meridian sun strikes the upper impenetrable foliage of my trees, and but a thousand.',
            name: 'Michkel Anegl',
            position: 'Marketing Management'
          },
          {
            url: 'fabio-spinelli-695744-unsplash-1024x1024.png',
            vote: 3,
            text: 'When, while lovely valley teems with vapor around meand meridian sun strikes the upper impenetrable foliage of my trees, and but a thousand.',
            name: 'Michkel Anegl',
            position: 'Marketing Management'
          },
        ],
        clients: [
          {
            url: 'client-1-1.png'
          },
          {
            url: 'client-5.png'
          },
          {
            url: 'clienty-2.png'
          },
          {
            url: 'clienty-3.png'
          },
          {
            url: 'clienty-4.png'
          },
        ]
      }
    }
}
</script>

<style scoped lang="scss">
@import '../../assets/style/general.scss';
.ms_section_offer {
  height: 150px;
  background-color: $textRed;
}
</style>