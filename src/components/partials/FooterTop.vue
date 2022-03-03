<template>
  <div class="container">
      <div class="row">
          <div class="col">
              <div>
                  <img src="../../assets/img/white-logo-2.png" alt="logo azienda">
              </div>
              <p>When, while lovely valley teems vapour aroundmeand meridian sun strikes the upper impenetrable</p>
          </div>
          <div class="col">
              <ul>
                  <li v-for="(link,index) in quickLinks" :key="index">{{link.text}}</li>
              </ul>
          </div>
          <div class="col">
              <ul>
                  <li v-for="(resource, index) in resources" :key="index">{{resource.text}}</li>
              </ul>
          </div>
          <div class="col">
              <h4>contact us</h4>
              <div><span>address: </span>patricia c. amedee 4401 waldeck street grapevine nashville, tx 76051</div>
              <div><span>phone: </span>+99 (0) 101 0000 888</div>
              <div><span>email: </span>info@yourdomain.com</div>
          </div>
      </div>
  </div>
</template>

<script>
export default {
    name: 'FooterTop',
    props: {
      'quickLinks': Array,
      'resources': Array
    }
}
</script>

<style scoped lang="scss">

</style>