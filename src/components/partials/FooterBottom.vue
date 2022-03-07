<template>
  <div class="container">
      <div class="row py-3">
          <div class="col-8">
              <span><i class="fa-solid fa-copyright pe-1"></i>2020 Phlox. All Right Reserved.</span>
          </div>
          <div class="col-3 text-end">
              <a href="#"><i class="fa-brands fa-instagram"></i></a>
              <a href="#"><i class="fa-brands fa-linkedin"></i></a>
              <a href="#"><i class="fa-brands fa-facebook"></i></a>
              <a href="#"><i class="fa-brands fa-twitter"></i></a>
          </div>
          <div class="col-1">
              <a href="#"><i class="fa-solid fa-comment"></i></a>
          </div>
      </div>
  </div>
</template>

<script>
export default {
    name: 'FooterBottom'
}
</script>

<style scoped lang="scss">
.container {
    border-top: 1px solid lightgray;
    span {
        font-size: 12px;
        color: #aaaaaa;
        font-weight: 100;
    }
    a {
        i {
            color: #fff;
            font-size: 12px;
            margin-right: 15px;
        }
    }
    .fa-comment {
        padding: 10px;
        border-radius: 50%;
        background-color: #527ceb;
    }
}

</style>