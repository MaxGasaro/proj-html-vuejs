<template>
<div id="header_top">
  <div class="container">
      <div class="row ms_row_header justify-content-center">
          <div class="col">
              <img src="../../assets/img/white-logo-2.png" alt="logo azienda">
          </div>
          <div class="col text-end d-flex align-items-center">
              <nav>
                  <ul>
                      <li v-for="(item, index) in itemsNav" :key="index"><a :href="item.url">{{item.text}}</a></li>
                  </ul>
              </nav>
          </div>
          <div class="col-2 text-end">
            <ButtonBlue message="Sign In"/>
          </div>
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
@import '../../assets/style/variables.scss';
#header_top {
    height: 50px;
    .ms_row_header {
        ul {
            list-style: none;
            display: flex;
            li {
                margin: 0 1rem;
                a {
                    text-decoration: none;
                    color: #fff;
                    padding: 0 5px;
                    font-size: 12px;
                    &:hover {
                        color: $textRed;
                    }
                }
            }
        }
    }
}
</style>