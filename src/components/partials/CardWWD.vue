<template>
  <div class="col px-4 ms_card my-4">
      <img :src="require(`../../assets/img/${card.img}`)">
      <div class="text_up text-center py-3">
          {{card.title}}
      </div>
      <div class="text_down text-center py-3">
          {{card.paragraph}}
      </div>
  </div>
</template>

<script>
export default {
    name: 'CardWWD',
    props: {
        'card': Object
    }
}
</script>

<style scoped lang="scss">
img {
    object-fit: contain;
    object-position: center;
    width: 50%;
    height: 50%;
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