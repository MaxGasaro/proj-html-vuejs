<template>
  <button class="d-flex justify-content-center align-items-center">{{message}}</button>
</template>

<script>
export default {
    name: 'ButtonBlue',
    props: {
        'message': String
    }
}
</script>

<style scoped lang="scss">
@import '../../assets/style/variables.scss';
button {
    padding: 10px 25px;
    border-radius: 20px;
    background: radial-gradient(circle at 120.71% 50%, #ffa279 0, #ff987a 8.33%, #ff8c7c 16.67%, #ff807e 25%, #ff7281 33.33%, #fa6385 41.67%, #f25389 50%, #e8438f 58.33%, #dd3696 66.67%, #cf2d9f 75%, #bf2baa 83.33%, #ac2db4 91.67%, #9534bf 100%);
    color: $primaryText;
    border: none;
    font-size: 0.8rem;
}
</style>