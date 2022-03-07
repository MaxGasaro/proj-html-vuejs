<template>
  <div id="translate" class="col">
      <div class="card text-center" :class="item.color?'card_red':''">
          <div class="fs-2 fw-bolder ms_zindex pt-3">{{item.title}}</div>
          <div class="fs-6 ms_zindex">{{item.subtitle}}</div>
          <div class="mt-4 price ms_zindex"><span>$</span>{{item.price}}</div>
          <div class="pb-5 fs-6 fw-light">{{item.period}}</div>
          <div class="fs-6 fw-light"><span class="fw-bold">{{item.span1}}</span> {{item.text1}}</div>
          <div class="py-2 fs-6 fw-light"><span class="fw-bold">{{item.span2}}</span> {{item.text2}}</div>
          <div class="fs-6 fw-light"><span class="fw-bold">{{item.span3}}</span> {{item.text3}}</div>
          <div class="py-2 fs-6 fw-light"><span class="fw-bold">{{item.span4}}</span> {{item.text4}}</div>
          <div class="fs-6 fw-light"><span class="fw-bold">{{item.span5}}</span> {{item.text5}}</div>
          <div><button :class="item.color?'button_white':'button'" class="my-5 rounded-pill">{{item.buttonContent}}<span class="ps-5"><i class="fa-solid fa-arrow-right-long"></i></span></button></div>
          <div class="number">
            {{item.price}}
          </div>
      </div>
  </div>
</template>

<script>
export default {
    name: 'CardPriceList',
    props: {
        'item': Object,
        'developing': String
    }
}
</script>

<style scoped lang="scss">
@import '../../assets/style/variables.scss';
#translate {
    transform: translateY(40%);
    .card_red {
        background: radial-gradient(circle at 120.71% 50%, #ffa279 0, #ff987a 8.33%, #ff8c7c 16.67%, #ff807e 25%, #ff7281 33.33%, #fa6385 41.67%, #f25389 50%, #e8438f 58.33%, #dd3696 66.67%, #cf2d9f 75%, #bf2baa 83.33%, #ac2db4 91.67%, #9534bf 100%);
        color: #fff;
    }
    .card {
        border-radius: 20px;
        position: relative;
        .ms_zindex {
            z-index: 999;
        }
        .price {
            font-size: 4.2rem;
            font-weight: 600;
            position: relative;
            span {
                font-weight: 300;
                font-size: 12px;
                position: absolute;
                top: 10px;
            }
        }
        .button_white {
            color: $textRed;
            background-color: #fff;
            padding: 5px 15px;
            font-weight: 600;
            border: none;
        }
        .button {
            padding: 5px 15px;
            font-weight: 600;
            color: #fff;
            background: radial-gradient(circle at 120.71% 50%, #ffa279 0, #ff987a 8.33%, #ff8c7c 16.67%, #ff807e 25%, #ff7281 33.33%, #fa6385 41.67%, #f25389 50%, #e8438f 58.33%, #dd3696 66.67%, #cf2d9f 75%, #bf2baa 83.33%, #ac2db4 91.67%, #9534bf 100%);
            border: none;
        }
        .number {
            font-size: 14rem;
            color: rgba($color: #000000, $alpha: 0.1);
            font-weight: 900;
            position: absolute;
            top: 0;
            right: 0;
            transform: translateY(-28%);
            z-index: 0;
        }
    }
}
</style>