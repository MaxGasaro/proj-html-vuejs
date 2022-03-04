<template>
  <div class="col g-4 ms_card my-4">
      <img src="../../assets/img/Group-247.png">
      <div class="text_up text-center py-3">
          {{textUp}}
      </div>
      <div class="text_down text-center py-3">
          When, while the lovely valley teems with vapour around meand the meridian sun strikes the upper
      </div>
  </div>
</template>

<script>
export default {
    name: 'CardWWD',
    props: {
        'textUp': String,
        'textDown': String
    }
}
</script>

<style scoped lang="scss">
img {
    object-fit: contain;
    object-position: center;
    width: 50%;
    transform: translateX(50%);
}
.text_up {
    font-size: 1.2rem;
    font-weight: 600;
}
.text_down {
    font-size: 12px;
}
</style>