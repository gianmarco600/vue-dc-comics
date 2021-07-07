<template>
    <main>
        <Jumbo/>
        <div class="container">
            <div class="row">
                <div class="label">current series</div>
                <ComicsCard
                     v-for="(card,index) in comicList" :key="index"
                     :comicObj="card"
                />
            </div>
            <div class="more">load more</div>
        </div>
    </main>
</template>

<script>
import Jumbo from '@/components/Jumbo.vue';
import ComicsCard from '@/components/ComicsCard.vue';
import dcComics from '@/assets/dcComics.js';

export default {
    name:'Main',
    components:{
        Jumbo,
        ComicsCard
    },
    data(){
        return{
            comicList: dcComics
        }
    }
}
</script>

<style lang="scss" scoped>
@import '@/style/vars.scss';
main{
    background-color: $background_dark;
    width: 100%;
    .container{
        width: 75%;
        margin: 0 auto;
        padding: 10px;
        text-align: center;
        h2{
            color:white;
            margin: 50px 0;
        }
        .row{
            position: relative;
            display: flex;
            flex-wrap: wrap;
            padding: 40px 0;
            .label{
                position: absolute;
                top: -40px;
                left: 0;
                display: inline-block;
                background-color: $primary;
                color: white;
                padding: 15px 20px;
                text-transform: uppercase;
                font-weight: 600;
                
            } 
        }
        .more{
            width: 300px;
            margin: 0 auto;
            padding: 20px 40px;
            margin: 40px 0;
            background-color: $primary;
            display: inline-block;
            color: white;
            text-transform: uppercase;
            cursor: pointer;
        }
        
    }
}

</style>