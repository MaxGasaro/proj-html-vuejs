<template>  
    <main>
        <WhatWeDo/>
        <SectionProject/>
        <LatestWorks/>
        <PriceList/>
    </main>
</template>

<script>
import LatestWorks from './partials/LatestWorks.vue'
import WhatWeDo from './partials/WhatWeDo.vue'
import SectionProject from './partials/SectionProject.vue'
import PriceList from './partials/PriceList.vue'

export default {
    name: 'MyMain',
    components: {
        LatestWorks,
        WhatWeDo,
        SectionProject,
        PriceList
    }

}
</script>

<style scoped lang="scss">

</style>