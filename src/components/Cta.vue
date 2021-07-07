<template>
    <div class="foot">
        <div class="container">
            <div class="row">
                <div class="btn"> <a>sign-up now!</a> </div>
                <div class="social">
                    <span>follow us</span>
                    <img src="@/assets/img/footer-facebook.png" alt="">
                    <img src="@/assets/img/footer-periscope.png" alt="">
                    <img src="@/assets/img/footer-pinterest.png" alt="">
                    <img src="@/assets/img/footer-twitter.png" alt="">
                    <img src="@/assets/img/footer-youtube.png" alt="">
                </div>
            </div>
            
        </div>
    </div>
</template>

<script>

export default {
    name:"Cta"
}
</script>

<style lang="scss" scoped>
@import '@/style/vars.scss';
.foot{
    width: 100%;
    background-color: #303030;
    .container{
        width: 75%;
        margin: 0 auto;
        height: 100%;
        padding: 40px 0;
        .row{
            display: flex;
            justify-content: space-between;
            align-items: center;
        
            .btn{
                width: 200px;
                padding:20px 15px;
                border: 2px solid $primary;
                display: flex;
                justify-content: center;
                align-items: center;
                cursor: pointer;
                a{
                    color: white;
                    display: block;
                    text-transform: uppercase;
                    font-weight: 500;
                }
                
            }
            .social{
                display: flex;
                justify-content: space-around;
                align-items: center;
                span{
                    margin: 0 20px;
                    color:$primary;
                    text-transform: uppercase;
                    font-weight: 500;
                }
                img{
                    margin: 0 8px;
                    cursor: pointer;
                }
            }
        }
    }
}

</style>