<template>
    <header>
        <div class="navbar">
            <div class="navbar_logo">
                <img src="../assets/dc-logo.png" alt="DC logo">
            </div>
            <div class="divider_div"></div>
            <ul class="navbar-list">
                <li class="navbar-list-item" v-for="(item, i) in navbarListItems" :key="i">
                    <a href="#" class="navbar-link " :class="i === 1 ? 'active' : ''">{{ item.title }}</a>
                </li>
            </ul>
        </div>
    </header>
</template>

<script>
export default {
    name: 'Header',
    data() {
        return {
            navbarListItems: [ 
                {
                    title: "Characters",
                },
                {
                    title: "Comics",
                },
                {
                    title: "Movies",
                },
                {
                    title: "Tv",
                },
                {
                    title: "Games",
                },
                {
                    title:  "Collectibles",
                },
                {
                    title: "Videos",
                },
                {
                    title: "Fans",
                },
                {
                    title: "News",
                },
                {
                    title: "Shop"
                },  
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../styles/header.scss";
</style>