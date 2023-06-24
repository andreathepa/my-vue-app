<script>
import AppComics from './AppComics.vue'

export default {
    components:{
    AppComics
  }
}
</script>

<template lang="">
    <div>
        <div class="jumbotron">
            <img src="../assets/img/jumbotron.jpg" alt="">
        </div>
        <div class="prova padding">
            <AppComics />
        </div>
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
        background-color: black;
    }

    
</style>