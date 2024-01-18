<script>
export default {
    data() {
        return {
            imageArray: [
                {
                    img: '/vue-dc-comics-1/img/buy-comics-digital-comics.png',
                    text: 'DIGITAL'
                },
                {
                    img: '/vue-dc-comics-1/img/buy-comics-merchandise.png',
                    text:'DC MERCHANDISE'
                },
                {
                    img: '/vue-dc-comics-1/img/buy-comics-shop-locator.png',
                    text:'SUBSCRIPTION'
                },
                {
                    img: '/vue-dc-comics-1/img/buy-comics-subscriptions.png',
                    text:'COMIC SHOP LOCATOR'
                },
                {
                    img: '/vue-dc-comics-1/img/buy-dc-power-visa.svg',
                    text:'DC VISA'
                },
            ]
        };
    },
    methods: {

    }
}
</script>

<template>
    <main>
        <section class="comix--blueSection d-flex ">
            <div class="container d-flex align-self-center justify-content-center">
                <div class="container-img"
                    v-for="elem in imageArray" >
                    <img :src="elem.img" alt="" class="me-2">
                    <span class="me-5">

                        {{ elem.text }}
                        
                    </span>
                </div>
            </div>
        </section>
        <section class="heroes-background">
            
        </section>
    </main>
</template>

<style lang="scss" scoped>
     @use "../assets/scss/main.scss" as *;
</style>
