<script>
export default {
    name: "AppHero",
};
</script>
<template lang="">
  <div class="banner_container">
    <div class="container">
        <span class="current_series text-white">current series</span>
    </div>
  </div>
</template>
<style lang="scss" scoped>
@use "../styles/partials/variables" as *;

.banner_container {
    background-image: url(../assets/img/jumbotron.jpg);
    background-size: cover;
    background-repeat: no-repeat;
    height: 400px;
    position: relative;

    .current_series {
        display: inline-block;
        background-color: $blue_primary;
        padding: 10px 30px;
        font-size: 18px;
        text-transform: uppercase;
        font-weight: 800;
        position: absolute;
        bottom: -18px;
    }
}
</style>
