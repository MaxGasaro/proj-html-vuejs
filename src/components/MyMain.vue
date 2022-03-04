<template>  
    <main>
        <WhatWeDo/>
        <LatestWorks/>
    </main>
</template>

<script>
import LatestWorks from './partials/LatestWorks.vue'
import WhatWeDo from './partials/WhatWeDo.vue'
export default {
    name: 'MyMain',
    components: {
        LatestWorks,
        WhatWeDo
    }

}
</script>

<style scoped lang="scss">

</style>