<template>
    <main>
        <div class="container">
            <h2>contenuto</h2>
        </div>
    </main>
</template>

<script>
export default {
    name:'Main'
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
        h2{
            color:white;
            margin: 50px 0;
        }
    }
}

</style>