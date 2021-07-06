<template>
    <footer>
        <div class="container">
            <div class="row">
                <div class="col">
                    <ul v-for="(section,index) in sections" :key="index">{{section.label}}
                        <li v-for="(link,index) in section.links" :key="index" > <a href="#" >{{setion.link[index]}}</a></li>
                    </ul>
                </div>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    name:'Footer',
    data(){
        return{
            sections:[
                {   
                    label:'nomesec',
                    links:['voce1','voce2','voce3','voce4'],
                },
                {  
                    label:'nomesec',
                    link:['voce1','voce2'],
                },
                {
                    label:'nomesec',
                    link:['voce1','voce2'],
                },

            ]
                
                

        }
        }
        

    }

</script>

<style lang="scss" scoped>
@import '@/style/vars.scss';
footer{
    background-image: url('../../public/img/footer-bg.jpg');
    width: 100%;
    height: 500px;
    .container{
        width: 75%;
        margin: 0 auto;
        .row{
            display: flex;
            justify-content: flex-start;
            padding: 70px 0;
            color: white;
            .col{
                width: 30%;
            }
        }
    }
}

</style>