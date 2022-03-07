<template>
  <div class="container">
      <div class="row">
          <div class="col">
              <div>
                  <img src="../../assets/img/white-logo-2.png" alt="logo azienda">
              </div>
              <p class="py-4 ms_12">When, while lovely valley teems vapour aroundmeand meridian sun strikes the upper impenetrable</p>
          </div>
          <div class="col">
              <ul>
                  <li class="ms_title_link fs-6 fw-bold pt-0">Quick Links</li>
                  <li v-for="(link,index) in quickLinks" :key="index"><a :href="link.url">{{link.text}}</a></li>
              </ul>
          </div>
          <div class="col">
              <ul>
                  <li class="ms_title_link fs-6 fw-bold pt-0">Resources</li>
                  <li v-for="(resource, index) in resources" :key="index"><a :href="resource.url">{{resource.text}}</a></li>
              </ul>
          </div>
          <div class="col ms_contact">
              <h4 class="fs-6 fw-bold text-capitalize">contact us</h4>
              <div class="py-3"><span>address: </span>patricia c. amedee 4401 waldeck street grapevine nashville, tx 76051</div>
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
.container {
    padding-top: 150px;
    ul {
        list-style: none;
        li {
            font-size: 12px;
            padding: 5px 0;
            a {
                color: #aaaaaa;
                font-weight: 100;
                text-decoration: none;
                &:hover {
                    color: #fff;
                }
            }
        }
    }
    .ms_12 {
        font-size: 12px;
    }
    p {
        color: #aaaaaa;
        font-weight: 100;
    }
    .ms_contact {
        div {
            color: #aaaaaa;
            font-size:12px;
            text-transform: capitalize;
            font-weight: 100;
            span {
                font-weight: 600;
                color: #fff;
            }
        }
    }
}

</style>