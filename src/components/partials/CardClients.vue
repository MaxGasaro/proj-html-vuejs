<template>
  <div class="col d-flex align-items-center justify-content-center">
      <img :src="require(`../../assets/img/${client.url}`)">
  </div>
</template>

<script>
export default {
    name: 'CardClients',
    props: {
        'client': Object
    }
}
</script>

<style scoped lang="scss">

</style>