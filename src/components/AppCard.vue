<script>
export default {
    props:{
        image: String,
        title: String,
        type: String,
        price: Number,
    }
}
</script>
<template lang="">
    <div class="card">
        <img :src="image" alt="">
        <h4>{{ title }}</h4>
        <p>{{ type }}</p>
        <p>{{ price }}</p>
    </div>
</template>
<style lang="scss" scoped>
    .card{
        width: calc(100% / 4);
        text-align: center; margin-bottom: 20px;
        transition: transform .2s;

        img{
            width: 200px;
            height: 300px;
        }

    }

    .card:hover{
        -ms-transform: scale(1.5);
        -webkit-transform: scale(1.5);
        transform: scale(1.5);
        background-color: rgba(0, 0, 0, 0.747);
        box-shadow: 1px 1px 50px#ffffff38;
    }

</style>