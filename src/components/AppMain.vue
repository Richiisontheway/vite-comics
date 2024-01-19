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
        <section class="heroes-background d-flex ">
            <div class="container d-flex">
                <div class="list-container">
                    <div class="list">
                        <h4>DC COMICS</h4>
                        <ul>
                            <li>Character</li>
                            <li>Comics</li>
                            <li>Movies</li>
                            <li>TV</li>
                            <li>Games</li>
                            <li>Videos</li>
                            <li>News</li>
                        </ul>
                    </div>
                    <div>
                        <h4>Shop</h4>
                        <ul>
                            <li>Shop DC</li>
                            <li>Shop DC Collectibles</li>
                        </ul>
                    </div>
                </div>
                <div class="list-container">
                    <h4>DC</h4>
                    <ul>
                        <li>Terms of use</li>
                        <li>Privacy Policy</li>
                        <li>Add Choise</li>
                        <li>Adverserting</li>
                        <li>Jobs</li>
                        <li>Subscrition</li>
                        <li>Talent Workshop</li>
                        <li>CPSC</li>
                        <li>Rating</li>
                        <li>Shop Help</li>
                        <li>Conctacs us</li>
                    </ul>
                </div>
                <div class="list-container">
                    <h4>Sites</h4>
                    <ul>
                        <li>Terms of use</li>
                        <li>Privacy Policy</li>
                        <li>Add Choise</li>
                        <li>Adverserting</li>
                    </ul>
                </div>
                <div class="d-flex align-items-center overflow-hidden ms-5">

                    <img src="/vue-dc-comics-1\img\dc-logo-bg.png" alt="">
                
                </div>
            </div>

        </section>
    </main>
</template>

<style lang="scss" scoped>
     @use "../assets/scss/main.scss" as *;
</style>
