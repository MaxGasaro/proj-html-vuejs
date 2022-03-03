<template>
  <div class="container">
      <div class="row ms_row_header justify-content-center">
          <div class="col">
              <img src="../../assets/img/white-logo-2.png" alt="logo azienda">
          </div>
          <div class="col">
              <nav>
                  <ul>
                      <li v-for="(item, index) in itemsNav" :key="index"><a :href="item.url">{{item.text}}</a></li>
                  </ul>
              </nav>
          </div>
          <div class="col">
            <ButtonBlue message="Sign In"/>
          </div>
      </div>
  </div>
</template>

<script>
import ButtonBlue from '../partials/ButtonBlue.vue'
export default {
    name: 'HeaderTop',
    props: {
        'itemsNav': Array
    },
    components: {
        ButtonBlue
    }
    
}
</script>

<style scoped lang="scss">
.ms_row_header {
    ul {
        list-style: none;
        display: flex;
        li {
            a {
                text-decoration: none;
                color: #fff;
            }
        }
    }
}
</style>