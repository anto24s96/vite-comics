<script>
export default {
    name: "AppCovers",
    props: {
        cover: Object
    }
}
</script>
<template lang="">
    <div class="card d-flex align-items">
        <div class="cover_container">
            <img :src="`${cover.thumb}`" alt="photos">
        </div>
        <span class="cover_title text-white">{{ cover.series }}</span>
    </div> 
</template>
<style lang="scss" scoped>
.card {
    margin: 10px;
    width: calc(100% / 6 - 20px);
    flex-direction: column;
    padding: px 0;

    .cover_container {
        height: 200px;
        width: 100%;

        img {
            height: 200px;
            object-fit: cover;
            object-position: top;
        }

    }

    .cover_title {
        text-transform: uppercase;
        display: inline-block;
        padding: 10px 0;
        font-weight: 600;
        text-align: center;
    }
}
</style>