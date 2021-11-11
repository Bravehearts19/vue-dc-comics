<template>
    <main>
        <div class="container_black">
            <h2>-->Content goes here--</h2>
        </div>

        <div class="container_blue">
            <ul>
                <li v-for="(option, i) in optionsClickList" :key="i">
                    <a href="#">
                        <div class="image_container">
                            <img :src="option.imgUrl" alt="">
                        </div>
                        <p>{{ option.textOption }}</p>
                    </a>
                </li>
            </ul>
        </div>
    </main>
</template>

<script>
export default {
    name: 'Main',
    data() {
        return {
            optionsClickList: [
                {
                    imgUrl: "../assets/buy-comics-digital-comics.png",
                    textOption: "Digital Comics",
                },
                {
                    imgUrl: "../assets/buy-comics-merchandise.png",
                    textOption: "DC Merchandise",
                },
                {
                    imgUrl: "../assets/buy-comics-subscribtions.png",
                    textOption: "Subscribtion",
                },
                {
                    imgUrl: "../assets/buy-comics-shop-locator.png",
                    textOption: "Comics Shop Locator",
                },
                {
                    imgUrl: "../assets/buy-dc-power-visa.svg",
                    textOption: "DC Power VISA",
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../styles/main.scss";
</style>