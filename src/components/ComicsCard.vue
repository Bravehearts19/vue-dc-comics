<template>
    <div class="comics_card">
        <div class="comics_card_image">
            <img :src="img" alt="">
        </div>
        <div class="comics_card_title">
            <h4>
                {{ title }}
            </h4>
        </div>
    </div>
</template>

<script>
export default {
    name: 'ComicsCard',
    props: {
        img: String,
        title: String
    }
}
</script>

<style lang="scss" scoped>
@import "../styles/main.scss";
</style>