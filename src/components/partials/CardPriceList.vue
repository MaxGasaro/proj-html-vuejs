<template>
  <div id="translate" class="col">
      <div class="card text-center">
          <div class="fs-2 fw-bolder">{{item.title}}</div>
          <div class="fs-6">{{item.subtitle}}</div>
          <div class="price"><span>$</span>{{item.price}}</div>
          <div class="fs-6 fw-light">{{item.period}}</div>
          <div class="fs-6 fw-light"><span class="fw-bold">{{item.span1}}</span> {{item.text1}}</div>
          <div class="fs-6 fw-light"><span class="fw-bold">{{item.span2}}</span> {{item.text2}}</div>
          <div class="fs-6 fw-light"><span class="fw-bold">{{item.span3}}</span> {{item.text3}}</div>
          <div class="fs-6 fw-light"><span class="fw-bold">{{item.span4}}</span> {{item.text4}}</div>
          <div class="fs-6 fw-light"><span class="fw-bold">{{item.span5}}</span> {{item.text5}}</div>
          <div><button class="button rounded-pill">{{item.buttonContent}}<span class="ps-5"><i class="fa-solid fa-arrow-right-long"></i></span></button></div>
      </div>
  </div>
</template>

<script>
export default {
    name: 'CardPriceList',
    props: {
        'item': Object
    }
}
</script>

<style scoped lang="scss">
#translate {
    transform: translateY(40%);
    .card {
        border-radius: 20px;
        .price {
            font-size: 5rem;
            font-weight: 600;
            span {
                font-weight: 300;
                font-size: 12px;
            }
        }
        .button {
            padding: 5px 15px;
            font-weight: 600;
            color: #fff;
            background: radial-gradient(circle at 120.71% 50%, #ffa279 0, #ff987a 8.33%, #ff8c7c 16.67%, #ff807e 25%, #ff7281 33.33%, #fa6385 41.67%, #f25389 50%, #e8438f 58.33%, #dd3696 66.67%, #cf2d9f 75%, #bf2baa 83.33%, #ac2db4 91.67%, #9534bf 100%);
        }
    }
}
</style>