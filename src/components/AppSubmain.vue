<script>
export default {
    name: "AppSubmain",
    data() {
        return {

        }
    },
}
</script>
<template lang="">
    <div class="bg-cian">
        <div class="container">
            <ul class="d-flex">
                <li class="d-flex">
                    <img src="../assets/img/buy-comics-digital-comics.png" alt="digital_comics" class="submain_images">
                    <span class="text-white">digital comics</span>
                </li>
                <li class="d-flex">
                    <img src="../assets/img/buy-comics-merchandise.png" alt="merchandise" class="submain_images">
                    <span class="text-white">dc merchandise</span>
                </li>
                <li class="d-flex">
                    <img src="../assets/img/buy-comics-subscriptions.png" alt="subscrition" class="submain_images">
                    <span class="text-white">subscrition</span>
                </li>
                <li class="d-flex">
                    <img src="../assets/img/buy-comics-shop-locator.png" alt="shop_locator" class="submain_images">
                    <span class="text-white">comic shop locator</span>
                </li>
                <li class="d-flex">
                    <img src="../assets/img/buy-dc-power-visa.svg" alt="dc_power_visa" class="submain_images">
                    <span class="text-white">dc power visa</span>
                </li>
            </ul>
        </div>
    </div>
</template>
<style lang="scss" scoped>
.bg-cian {
    background-color: #0282F9;

    ul {
        list-style-type: none;
        justify-content: space-between;
        padding: 50px;

        li {
            align-items: center;

            .submain_images {
                width: 45px;
                margin-right: 10px;
            }

            span {
                text-transform: uppercase;
            }
        }
    }
}
</style>