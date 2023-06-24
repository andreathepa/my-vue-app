<script>
export default {
    props:{
        image: String,
        title: String,
        type: String,
        price: Number
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
        text-align: center;

        img{
            width: 200px;
        }
    }
</style>