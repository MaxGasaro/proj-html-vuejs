<template>
  <section id="latestpost">
    <InitSectionCenter
    sectionName="Blog"
    title="Posts"
    titleBolder="Latest"
    paragraph="When, while the lovely valley teems with vapour around meand the meridian sun strikes the upper surface"
    />
    <div class="container py-5">
        <div class="row justify-content-center">
            <div class="col-6 ms_big_col text-white d-flex flex-column justify-content-end p-5">
                <div class="date ms_12px">April 21,2019 <i class="fa-solid fa-period"></i> by Paul</div>
                <div class="fw-bolder pt-3">Amazon gets CCI nod to acquire 49% stake in</div>
                <div class="d-flex justify-content-between pt-3">
                    <div class="w-75 ms_12px">When, while the lovely valley teems with vapor around me, and the meridian sun s...</div>
                    <button class="readmore">Read More</button>
                </div>
            </div>
            <div class="col-3 ms_small_col text-white d-flex flex-column justify-content-end p-5">
                <div class="date ms_12px">April 21,2019 <i class="fa-solid fa-period"></i> by Paul</div>
                <div class="fw-bolder pt-4">Clearing Corporations get SEBI nod to invest in overnight funds</div>
                <div class="pt-4">
                    <div class="pb-4 ms_12px">When, while the lovely valley teems with vapor around me, and the meridian sun s...</div>
                    <button class="readmore">Read More</button>
                </div>
            </div>
            <div class="col-3 ms_small_col text-white d-flex flex-column justify-content-end p-5">
                <div class="date ms_12px">April 21,2019 <i class="fa-solid fa-period"></i> by Paul</div>
                <div class="fw-bolder pt-4">Shabnam Dhillion, wife of RSSB chief Gurinder Dhillon, passes away in London</div>
                <div class="pt-4">
                    <div class="pb-4 ms_12px">When, while the lovely valley teems with vapor around me, and the meridian sun s...</div>
                    <button class="readmore">Read More</button>
                </div>
            </div>
        </div>
    </div>

  </section>
</template>

<script>
import InitSectionCenter from './InitSectionCenter.vue'
export default {
    name: 'LatestPost',
    components: {
       InitSectionCenter 
    }
}
</script>

<style scoped lang="scss">
@import '../../assets/style/general.scss';
#latestpost {
    .ms_big_col {
        background-image: url('../../assets/img/headway-537308-unsplash-1380x703.jpg');
        background-size: cover;
        height: 400px;
        border-radius:20px;
        
    }
    .ms_small_col {
        height: 400px;
        background: linear-gradient(151deg, rgba(13,5,145,1) 0%, rgba(9,9,121,1) 40%, rgba(0,143,255,1) 100%);
        border-radius:20px;
    }
    .ms_12px {
        font-size: 12px;;
    }
}

</style>