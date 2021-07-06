<template>
    <footer>
        <div class="container">
            <div class="row">
            <div class="col"></div>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    name:'Footer'
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
    }
}

</style>