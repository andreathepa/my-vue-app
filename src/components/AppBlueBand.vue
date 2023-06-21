<script>
export default {
    data(){
        return{
            icons: 
            [
                {
                    title: 'DIGITAL COMICS',
                    icona: "./src/assets/img/buy-comics-digital-comics.png",
                    active: false,
                },
                {
                    title: 'DC MERCHANDISE',
                    icona: "./src/assets/img/buy-comics-merchandise.png",
                    active: false,
                },
                {
                    title: 'SUBSCRIPTION',
                    icona: "./src/assets/img/buy-comics-subscriptions.png",
                    active: false,
                },
                {
                    title: 'COMIC SHOP LOCATOR',
                    icona: "./src/assets/img/buy-comics-shop-locator.png",
                    active: false,
                },
                {
                    title: 'DC POWER VISA',
                    icona: "./src/assets/img/buy-dc-power-visa.svg",
                    active: false,
                },
            ]
        };
    },
    
}
</script>

<template lang="">
    <div>
        <div class="container_icons">
            <div class="footer_blue flex justify-content-between align-items-center">
                 <a class="flex align-items-center margin-left" v-for="(icon, index) in icons" :key="index" href="#">

                    <div class="image_icon"><img :src="icon.icona" alt=""></div>
                    <div class="align-items-center margin-left">{{ icon.title }}</div>
                 </a>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>

    .container_icons{
        background-color: rgb(66, 100, 253);
        
        .footer_blue{
            height: 150px;
            margin: 0 auto;
            max-width: 1300px;
            color:white;
        }

        a{
            color: rgb(255, 255, 255);
        }
        img{
            width: 60px;
        }

    }

</style>