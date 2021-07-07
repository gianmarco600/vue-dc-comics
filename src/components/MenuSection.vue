<template>
    <section>
        <div class="container">
            <div class="row">
                <div v-for="(link,index) in links" :key="index" class="col">
                    <img  :src='getImg(link.image)' alt="ciao">
                    <h3>{{link.text}}</h3>
                </div>
            </div>
        </div>
    </section>
</template>

<script>

export default {

    name:'MenuSection',
    data(){
        return{
            links:[
                {
                    text: 'digital comics',
                    image: 'buy-comics-digital-comics.png'
                    

                },
                {
                    text: 'dc merchandise',
                    image: 'buy-comics-merchandise.png'
                    
                },
                {
                    text: 'subscription',
                    image: 'buy-comics-shop-locator.png'
                     
                },
                {
                    text: 'comic shop locator',
                    image: 'buy-comics-subscriptions.png'
                     
                },
                {
                    text: 'dc power visa',
                    image: 'buy-dc-power-visa.svg'
                    
                },

            ]
        }
    },
    methods:{
        getImg(img){
            return require('@/assets/img/' + img )
        }
    }
}
</script>

<style lang="scss" scoped>
@import '@/style/vars.scss';
section{
    background-color: $primary;
    width: 100%;
    .container{
        width: 75%;
        margin: 0 auto;
        
        .row{
            display: flex;
            justify-content: space-around;
            height: 130px;
            .col{
                display: flex;
                align-items: center;
                justify-content: center;
                cursor: pointer;
                width: calc(100% / 5);
                &:hover{
                    background-color: #0572d8;
                }
                h3{
                    display: inline-block;
                    margin-left: 5px;
                    font-size: 18px;
                    font-weight: 300;
                    color: white;
                    text-transform: uppercase;
                }
                img{
                    display: block;
                    width: 40px;
                }
                
                
                
            }
        }
    }
}

</style>