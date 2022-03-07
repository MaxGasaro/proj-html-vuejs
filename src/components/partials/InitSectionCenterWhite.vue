<template>
<div class="text-center my-4">
  <div class="ms_little_title_red text-center">{{sectionName}}</div>
  <div class="ms_title_section text-center text-white py-2"><span class="ms_title_bolder">{{titleBolder}}</span> {{title}}</div>
  <div class="ms_paragraph_section text-center text-white">{{paragraph}}</div>
</div>
</template>

<script>
export default {
    name: 'InitSectionCenter',
    props: {
        'sectionName': String,
        'title': String,
        'titleBolder': String,
        'paragraph': String,
    }
}
</script>

<style scoped lang="scss">
@import '../../assets/style/general.scss';
.ms_title_section {
    text-transform: capitalize;
    font-size: 1.5rem;
    font-weight: 400;
    .ms_title_bolder {
        font-weight: 600;
    }
}
.ms_paragraph_section {
    font-size: 12px;
}

</style>