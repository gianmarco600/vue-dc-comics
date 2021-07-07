<template>
    <footer>
        <div class="container">
            <div class="row">
                <div class="col">
                    <ul>
                        <h4>dc comics</h4>
                        <li> <a href="#">Characters</a></li>
                        <li> <a href="#">Comics</a></li>
                        <li> <a href="#">Movies</a></li>
                        <li> <a href="#">TV</a></li>
                        <li> <a href="#">Games</a></li>
                        <li> <a href="#">Videos</a></li>
                        <li> <a href="#">News</a></li>
                    </ul>
                    <ul>
                        <h4>shop</h4>
                        <li> <a href="#">Shop DC</a></li>
                        <li> <a href="#">Shop DC Collectibles</a></li>
                    </ul>
                    <ul>
                        <h4>DC</h4>
                        <li> <a href="#">term of use</a></li>
                        <li> <a href="#">privacy policy (new)</a></li>
                        <li> <a href="#">ad choices</a></li>
                        <li> <a href="#">advertising</a></li>
                        <li> <a href="#">jobs</a></li>
                        <li> <a href="#">subscriptions</a></li>
                        <li> <a href="#">talent workshops</a></li>
                        <li> <a href="#">CPSC certificates</a></li>
                        <li> <a href="#">ratings</a></li>
                        <li> <a href="#">shop help</a></li>
                        <li> <a href="#">contact us</a></li>
                    </ul>
                    <ul>
                        <h4>sites</h4>
                        <li> <a href="#">DC</a></li>
                        <li> <a href="#">MAD magazine</a></li>
                        <li> <a href="#">DC kids</a></li>
                        <li> <a href="#">DC universe</a></li>
                        <li> <a href="#">DC power visa</a></li>
                    </ul>
                </div>
            </div>
            
        </div>
        <Cta/>
    </footer>
</template>

<script>

import Cta from '@/components/Cta.vue';

export default {
    name:'Footer',
    components:{
        Cta
    },
    data(){
        return{
            
                
                

        }
        }
        

    }

</script>

<style lang="scss" scoped>
@import '@/style/vars.scss';
footer{
    background-image: url('../assets/img/footer-bg.jpg');
    background-size: cover;
    background-repeat: no-repeat;
    width: 100%;
    height: 500px;
    .container{
        width: 75%;
        margin: 0 auto;
        height: 100%;
        .row{
            display: flex;
            justify-content: flex-start;
            padding: 70px 0;
            color: white;
            height: 100%;
            .col{
                width: 30%;
                display: flex;
                flex-direction: column;
                flex-wrap: wrap;
                ul{
                    margin-right:30px;
                    text-transform: uppercase;
                    list-style: none;
                    h4{
                        font-size: 20px;
                        font-weight: 500;
                        margin: 15px 0 ;

                    }
                    a{
                    text-transform: capitalize;
                    color: white;
                    text-decoration: none;
                    font-size: 14px;
                    margin: 5px 0;
                    font-weight: 300;
                    
                }
                }
                
            }
        }
    }
}

</style>