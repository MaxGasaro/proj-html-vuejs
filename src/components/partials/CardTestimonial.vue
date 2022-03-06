<template>
  <div class="col text-center ms_text">
      <img :src="require(`../../assets/img/${testimonial.url}`)">
      <div class="py-4">{{testimonial.vote}}</div>
      <div class="pb-4">{{testimonial.text}}</div>
      <div class="pb-1 fw-bolder">{{testimonial.name}}</div>
      <div class="fw-lighter">{{testimonial.position}}</div>
  </div>
</template>

<script>
export default {
    name: 'CardTestimonial',
    props: {
        'testimonial': Object
    }
}
</script>

<style scoped lang="scss">
@import '../../assets/style/variables.scss';
img {
    width: 50px;
    height: 50px;
    border-radius: 50%;
    border: 2px solid $textRed;
}
.ms_text {
    font-size: 12px;
}
</style>