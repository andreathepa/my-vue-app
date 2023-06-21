<script>
export default {
    data(){
        return{
            links: 
            [
                {
                    label: 'Voce 1',
                    href: '#',
                    active: false,
                },
                {
                    label: 'Voce 2',
                    href: '#',
                    active: false,
                },
                {
                    label: 'Voce 3',
                    href: '#',
                    active: false,
                },
                {
                    label: 'Voce 4',
                    href: '#',
                    active: false,
                }
            ]
        };
    }

}
</script>

<template>
    <header class="container">
        <div class="flex justify-content-between">
            <img src="/dc-logo.png" alt="">
            <nav>
                <ul>
                    <li v-for="(link, index) in links" :key="index">
                        <a :href="link.href" :active="link.active ? 'active' : ''">
                            {{ link.label }}
                        </a>
                    </li>
                </ul>
            </nav>

        </div>
    </header>
</template>

<style lang="scss" scoped>
    @use '../styles/partials/variables' as *;

    .active{
        border-bottom: 2px solid blue;
    }

    header{
        padding: 20px 0px;

        ul li{
        display: inline-block;
        padding: 30px 20px;
        
            a{
                font-size: 20px;
                font-weight: 600px;
            }

            &:hover a{
                color: blue;
        
            }
            
            &:hover{
                border-bottom: 2px solid blue;
            }
    }
    
    }

    
</style>