<template>
    <header>
        <div class="top_header"></div>
        <nav>
            <div class="menu">
                <div id="logo"><a href="#"><img src="@/assets/img/dc-logo.png" alt=""></a></div>
                <div class="nav_menu">
                    <div class="menu_elem"><a href="#">esargbvwet</a></div>
                    <div class="menu_elem"><a href="#">esarvgsbg</a></div>
                    <div class="menu_elem"><a href="#">asdsdfbvsd</a></div>
                    <div class="menu_elem"><a href="#">aasdagadfg</a></div>
                    <div class="menu_elem"><a href="#">aasdasd</a></div>
                    <div class="menu_elem"><a href="#">asdfaa</a></div>
                    <div class="menu_elem"><a href="#">asdfaa</a></div>
                    <div class="menu_elem"><a href="#">avasdaf</a></div>
                    <div class="menu_elem"><a href="#">a vfdas</a></div>
                    <div class="menu_elem"><a href="#">avsadfgv</a></div>
                </div>    
            </div>
        </nav>
    </header>
</template>

<script>
export default {
    name:"Header"
}
</script>

<style lang="scss" scoped>
@import '@/style/vars.scss';
header{
    width: 100%;
    .top_header{
        background-color: $background_dark;
        height: 50px;
    }
    nav{
        width: 80%;
        margin: 0 auto;
        padding: 20px;

        .menu{
            display: flex;
            justify-content: space-between;
            align-content: center;

            .nav_menu{
                display: flex;
                align-content: center;

                .menu_elem{
                    height: 100%;
                    display: flex;
                    height: 100px;
                    align-content: center;
                    padding: 15px;
                    
                    vertical-align: middle;
                    &:hover{
                        background-color: aqua;
                    }
                    
                }
            }
                
        }

    }
}
</style>