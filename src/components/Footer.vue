<template>
    <footer>
        <div class="container_dc">
            <div class="lists_container">
                <ul v-for="(list, i) in footerLists" :key="i">
                    <li>
                        <h1> {{ list.title }} </h1>
                    </li>
                    <li v-for="(text, index) in list.links" :key="index">
                        <a href="#">{{ text }}</a>
                    </li>
                </ul>
            </div>
            <div class="divider_div"></div>
            <div class="image_container">
                <img src="../assets/dc-logo-bg.png" alt="">
            </div>
        </div>

        <div class="last_container">
            <button type="button">SIGN UP NOW!</button>
            <div class="divider_div"></div>
            <ul>
                <li>
                    <a href="#">Follow us</a>
                </li>
                <li v-for="(image, i) in footerImageUrlList" :key="i">
                    <div class="image_container">
                        <img :src="image" alt="">
                    </div>
                </li>
            </ul>
        </div>
    </footer>
</template>

<script>
export default {
    name: 'Footer',
    data() {
        return {
            footerLists: [
                {
                    title: "DC Comics",
                    links: [
                        "Characters",
                        "Comics",
                        "Movies",
                        "Tv",
                        "Games",
                        "Videos",
                        "News"
                    ]
                },
                {
                    title: "Shop",
                    links: [
                        "Shop DC",
                        "Shop DC Collectibles"
                    ]
                },
                {
                    title: "DC",
                    links: [
                        "Terms of use",
                        "Privacy policy (New)",
                        "Ad Choices",
                        "Advertising",
                        "Jobs",
                        "Subscriptions",
                        "Talent Workshops",
                        "CPSC Certificates",
                        "Ratings",
                        "Shop help",
                        "Contact us"
                    ]
                },
                {
                    title: "Sites",
                    links: [
                        "DC",
                        "MAD Magazine",
                        "DC Kids",
                        "DC Univers",
                        "DC Power Visa",
                    ]
                },
            ],
            footerImageUrlList: [
                "../assets/footer-facebook.png",
                "../assets/footer-twitter.png",
                "../assets/footer-youtube.png",
                "../assets/footer-pinterest.png",
                "../assets/footer-periscope.png",
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../styles/footer.scss";
</style>