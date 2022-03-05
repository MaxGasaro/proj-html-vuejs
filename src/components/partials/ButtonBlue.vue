<template>
  <button>{{message}}</button>
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
    padding: 5px 15px;
    border-radius: 20px;
    background: radial-gradient(circle at -18.3% 68.3%, #e7ffff 0, #bcedff 16.67%, #8dd5fb 33.33%, #53bcf2 50%, #00a3e9 66.67%, #008be1 83.33%, #0075d9 100%);
    color: $primaryText;
    border: none;
}
</style>