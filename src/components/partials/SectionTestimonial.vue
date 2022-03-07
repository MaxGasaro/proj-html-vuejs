<template>
  <section id="testimonial">
      <InitSectionCenter
        sectionName="Testimonial"
        title="People Say"
        titleBolder="What"
        paragraph="When, while the lovely valley teems vapour around meand the meridian sun strikes the upper surface."
      />
      <div class="container py-5">
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
      <div class="container ms_section_offer p-5">
        <div class="row align-items-center h-100">
          <div class="col d-flex flex-column justify-content-center h-100">
            <div class="fs-2 fw-bolder">We Offer Awesome Services</div>
            <div class="ms_12">When, while lovely valley teems with vapour around meand meridian sun strikes the upper surface.</div>
          </div>
          <div class="col-4 text-end bg-white py-1 ps-5 rounded-pill">
            <div class="row">
              <div class="col-8 text-start d-flex align-items-center">
                <input class="border-0 fw-lighter" type="text" placeholder="Enter Your Email Address">
              </div>
              <div class="col-4 text-center">
                <ButtonBlue message="Subscribe"/>
              </div>
            </div>
          </div>
        </div>
      </div>
  </section>
</template>

<script>
import InitSectionCenter from './InitSectionCenter.vue'
import CardTestimonial from './CardTestimonial.vue'
import CardClients from './CardClients.vue'
import ButtonBlue from './ButtonBlue.vue'
export default {
    name: 'SectionTestimonial',
    components: {
        InitSectionCenter,
        CardTestimonial,
        CardClients,
        ButtonBlue
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
            vote: 5,
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
  background: radial-gradient(circle at 120.71% 50%, #ffa279 0, #ff987a 8.33%, #ff8c7c 16.67%, #ff807e 25%, #ff7281 33.33%, #fa6385 41.67%, #f25389 50%, #e8438f 58.33%, #dd3696 66.67%, #cf2d9f 75%, #bf2baa 83.33%, #ac2db4 91.67%, #9534bf 100%);
  transform: translateY(50%);
  border-radius: 30px;
  color: #fff;
  .ms_12 {
    font-size: 12px;
  }
}
</style>