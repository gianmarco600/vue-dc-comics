<template>
    <div class="card">
        <img :src="comicObj.thumb" :alt="comicObj.type">
        <div class="title">{{comicObj.series}}</div>
    </div>
</template>

<script>



export default {
    name:"ComicsCard",
    props:["comicObj"]

}
</script>

<style lang="scss">
.card{
    width: calc(100% / 6 - 20px);
    margin: 20px 10px;
    img{
        width: 100%;
        max-height: 250px;
        
        display: block;
    }
    .title{
        margin: 10px 0;
        padding: 0 10px;
        color: white;;
    }
    
}

</style>