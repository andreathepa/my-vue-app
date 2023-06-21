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
        <div class="footer_bg">
             <img src="../assets/img/footer-bg.jpg" class="bg_img" alt="">
             <img src="../assets/img/dc-logo-bg.png" class="bg_logo" alt="">
        </div>
        <div class="container_sign_up">
           <div class="sign_up flex justify-content-between align-items-center">
                <div class="">
                    <button class="">
                        SIGN-UP NOW!
                    </button>
                </div>
                <div>
                    <ul>
                        <li>FOLLOW US</li>
                        <li>ciao</li>
                        <li>ciao</li>
                        <li>ciao</li>
                        <li>ciao</li>
                    </ul>
                </div>
           </div> 

       </div>
    </div>
</template>

<style lang="scss" scoped>

    ul li{
        display: inline-block;
        padding: 30px 20px;
    }
    
    .footer_bg{
        position: relative;
        overflow: hidden;
        width: 100%;
        height: 50vh;

        .bg_img{
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 140%;
            object-fit: cover;
            
        }

        .bg_logo{
            height: 604px;
            position: absolute;
            top: -46px;
            right: 287px;
        }
        
    }

    .container_sign_up{
        background-color: rgb(37, 37, 37);

        .sign_up{
                height: 100px;
                margin: 0 auto;
                max-width: 1320px;
    
                button{
                    padding: 15px;
                    border: 1px solid blue;
                    cursor: pointer;
                    background-color: rgb(37, 37, 37) ;
                    color: white;
                }
    
                
            }

    }
</style>