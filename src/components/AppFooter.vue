<script>
export default {
    data(){
        return{
            socials: 
            [
                {
                    label: '',
                    href: '#',
                    logo_social: './src/assets/img/footer-facebook.png',
                    active: false,
                },
                {
                    label: '',
                    href: '#',
                    logo_social: './src/assets/img/footer-periscope.png',
                    active: false,
                },
                {
                    label: '',
                    href: '#',
                    logo_social: './src/assets/img/footer-pinterest.png',
                    active: false,
                },
                {
                    label: '',
                    href: '#',
                    logo_social: './src/assets/img/footer-twitter.png',
                    active: false,
                },
                {
                    label: '',
                    href: '#',
                    logo_social: './src/assets/img/footer-youtube.png',
                    active: false,
                }
            ]
        };
    }
    
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
                <div class="flex align-items-center">
                    <div class="follow"><a href="">FOLLOW US</a></div>
                    <ul>
                        <li v-for="(social, index) in socials" :key="index">
                        <a :href="social.href" :active="social.active ? 'active' : ''">
                            <div><img :src="social.logo_social" alt=""></div>
                        </a>
                    </li>
                    </ul>
                </div>
           </div> 

       </div>
    </div>
</template>

<style lang="scss" scoped>

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

        .follow{
            font-size: 25px;
            font-weight: 600;

            a{
                color: rgb(0, 89, 255);
            }

            a:hover{
                color: rgb(255, 255, 255);

            }

            
        }
        
        .active{
        border-bottom: 2px solid rgb(255, 255, 255);
        }

        ul li{
        display: inline-block;
        padding: 30px 20px;
        
            &:hover{
                background-color: rgba(255, 255, 255, 0.205);
                
            }

            
    }
    
    }

    
</style>