<template>  
    <main>
        <WhatWeDo/>
        <SectionProject/>
        <LatestWorks/>
        <PriceList/>
        <LatestPost/>
        <SectionTestimonial/>
    </main>
</template>

<script>
import LatestWorks from './partials/LatestWorks.vue'
import WhatWeDo from './partials/WhatWeDo.vue'
import SectionProject from './partials/SectionProject.vue'
import PriceList from './partials/PriceList.vue'
import LatestPost from './partials/LatestPost.vue'
import SectionTestimonial from './partials/SectionTestimonial.vue'

export default {
    name: 'MyMain',
    components: {
        LatestWorks,
        WhatWeDo,
        SectionProject,
        PriceList,
        LatestPost,
        SectionTestimonial
    }

}
</script>

<style scoped lang="scss">

</style>