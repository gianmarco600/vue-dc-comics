<template>
    <header>
        <nav>
            <div class="menu">
                <div id="logo"><a href="#"><img src="@/assets/img/dc-logo.png" alt=""></a></div>
                <div class="nav_menu">
                    <div v-for="(link,index) in links" :key="index" class="menu_elem" :class="link.current ? 'active' : ''" :href="link.url"><a :class="link.current ? 'active' : ''" :href="link.url" >{{link.text}}</a></div>
                    
                </div>    
            </div>
        </nav>
    </header>
</template>






<script>
export default {
    name:"Header",
    data(){
        return{
            links:[
                {
                    text:'characters',
                    url:'#',
                    current: false
                },
                {
                    text:'comics',
                    url:'#',
                    current: true
                },
                {
                    text:'movies',
                    url:'#',
                    current: false
                },
                {
                    text:'tv',
                    url:'#',
                    current: false
                },
                {
                    text:'games',
                    url:'#',
                    current: false
                },
                {
                    text:'collectibles',
                    url:'#',
                    current: false
                },
                {
                    text:'videos',
                    url:'#',
                    current: false
                },
                {
                    text:'fans',
                    url:'#',
                    current: false
                },
                {
                    text:'news',
                    url:'#',
                    current: false
                },
                {
                    text:'shop',
                    url:'#',
                    current: false
                }
            ]
        }
    }
}
</script>





<style lang="scss" scoped>
@import '@/style/vars.scss';
header{
    width: 100%;
    position: fixed;
    top: 0;
    z-index: 9999999;
    background-color: white;
    nav{
        width: 75%;
        margin: 0 auto;
        padding: 0px;
        

        .menu{
            display: flex;
            justify-content: space-between;
            align-items: center;
            #logo{
                a{
                    img{
                        height: 80px;
                    }
                }
            }
            .nav_menu{
                display: flex;
                align-content: center;

                .menu_elem{
                    height: 100%;
                    display: flex;
                    flex-direction: column;
                    height: 100px;
                    justify-content: center;
                    padding: 0 7px;
                    margin: 0 7px;
                    box-sizing: content-box;
                    a{
                        text-transform: uppercase;
                        text-decoration: none;
                        color: black;
                        display: inline-block;

                        
                    }
                    &:hover,
                    &.active{
                    border-bottom: 5px solid $primary;
                    color: $primary;
                    }
                    
                    
                }
            }
                
        }

    }
}
</style>