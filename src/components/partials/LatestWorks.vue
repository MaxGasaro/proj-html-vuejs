<template>
  <section id="latest_works">
      <div class="container">
          <div class="row">
              <div class="ms_little_title_red col">
                  Portfolio
              </div>
          </div>
          <div class="row justify-content-between">
              <div class="col">
                  <span>latest</span> work
              </div>
              <div class="col text-end">
                  <i class="fa-solid fa-arrow-left-long"></i>
                  <i class="fa-solid fa-arrow-right-long"></i>
              </div>
          </div>
      </div>
      <div class="container-fluid">
          <div class="row flex-nowrap ms_overflow g-5">
              <div class="col-3 ms_card">
                  <img src="../../assets/img/8wa60okr-1-790x576.jpg" alt="foto1">
                  <div class="d-flex justify-content-between">
                      <p>ciao</p>
                      <p>mondo</p>
                  </div>
              </div>
              <div class="col-3 ms_card">
                  <img src="../../assets/img/8wa60okr-1-790x576.jpg" alt="foto1">
                  <div class="d-flex justify-content-between">
                      <p>ciao</p>
                      <p>mondo</p>
                  </div>
              </div>
              <div class="col-3 ms_card">
                  <img src="../../assets/img/8wa60okr-1-790x576.jpg" alt="foto1">
                  <div class="d-flex justify-content-between">
                      <p>ciao</p>
                      <p>mondo</p>
                  </div>
              </div>
              <div class="col-3 ms_card">
                  <img src="../../assets/img/8wa60okr-1-790x576.jpg" alt="foto1">
                  <div class="d-flex justify-content-between">
                      <p>ciao</p>
                      <p>mondo</p>
                  </div>
              </div>
              <div class="col-3 ms_card">
                  <img src="../../assets/img/8wa60okr-1-790x576.jpg" alt="foto1">
                  <div class="d-flex justify-content-between">
                      <p>ciao</p>
                      <p>mondo</p>
                  </div>
              </div>
          </div>
          <div class="row justify-content-center">
              <div class="col d-flex justify-content-center">
                  <div 
                     v-for="n,index in 5" :key="index" class="active_check" :class="index=indice?'active':''">
                  </div>
              </div>
          </div>
      </div>
  </section>
</template>

<script>
export default {
    name: 'LatestWorks'
}
</script>

<style scoped lang="scss">
@import '../../assets/style/general.scss';
@import '../../assets/style/variables.scss';
#latest_works {
    .ms_overflow {
        overflow-x: auto;
        img {
            object-fit: contain;
            width: 100%;
        }
    }
    .active_check {
        width: 8px;
        height: 8px;
        border-radius: 50%;
        background-color: lightgray;
        margin: 8px 4px;
    }
    .active {
        background-color: red;
    }
}

</style>