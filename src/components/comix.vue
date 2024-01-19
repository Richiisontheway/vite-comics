
<script>
export default {
    data() {
        return {
            
        };
    },
    props : {
        img: String,
        name: String
    }
}
</script>

<template>
    <div class="col-2 comix--col ">
        <div class="comix--imgContainer">
            <img :src="img" alt="">
        </div>
        <h5>
            {{ name }}
        </h5>
    </div>
</template>

<style lang="scss">
.comix--col{
    height: 50vh;
    .comix--imgContainer{
    height: 250px;
    width: 200px;
    overflow: hidden;
    img{
        width: 100%;
    }
}
}
</style>


