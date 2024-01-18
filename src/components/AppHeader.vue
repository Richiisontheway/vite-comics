<script>
export default {
    data() {
        return {
            headerList: [
                {
                    name: 'characters'
                },
                {
                    name: 'comics'
                },
                {
                    name: 'movies'
                },
                {
                    name: 'tv'
                },
                {
                    name: 'games'
                },
                {
                    name: 'collectibles'
                },
                {
                    name: 'videos'
                },
                {
                    name: 'fans'
                },
                {
                    name: 'news'
                },
                {
                    name: 'shop'
                },
            ]
        };
    },
    methods: {

    }
}
</script>

<template>
    <header>
        <section class="d-flex align-items-center comix--headerContainer">
            <div class="container d-flex align-items-center justify-content-between">

                <div class="img-container">
                    <img src='/vue-dc-comics-1/img/dc-logo.png' alt="">
                </div>

                <ul>
                    <li v-for="elem in headerList">
                        {{ elem.name }}
                    </li>
                </ul>

            </div> 
        </section>
        <section class="comics--newText d-flex">
            <div class="container d-flex align-items-center ">
                --/ New Content Here /--
            </div>
        </section>
    </header>
</template>

<style lang="scss" scoped>
    @use "../assets/scss/header.scss" as *;
</style>
