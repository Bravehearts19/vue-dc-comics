<template>
    <footer>
        <div class="container_dc">
            <ul v-for="(list, i) in footerLists" :key="i">
                <li>
                    <h1> {{ list.title }} </h1>
                </li>
                <li v-for="(text, index) in list.links" :key="index">
                    <a href="#">{{ text }}</a>
                </li>
            </ul>
        </div>

        <div class="last_container">
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
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../styles/footer.scss";
</style>