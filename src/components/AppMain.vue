<script>
export default {

}
</script>

<template lang="">
    <div>
        <div class="jumbotron">
            <img src="../assets/img/jumbotron.jpg" alt="">
        </div>
        <div class="prova">Content blue goes here</div>
    </div>
</template>

<style lang="scss" scoped>
    .jumbotron{
        position: relative;
        overflow: hidden;
        width: 100%;
        height: 50vh;

        img{
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 200%;
            object-fit: cover;
            
        }
    }   
    .prova{
        height: 1000px;
        background-color: black;
    }

    
</style>