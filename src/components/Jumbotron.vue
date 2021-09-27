<template>
    <div id="jumbotron">
        <img src="../assets/images/jumbotron.jpg" alt="">
    </div>
</template>

<script>
export default {
    name : 'Jumbotron'
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";
@import "../style/general.scss";
    #jumbotron{
        height: 500px;

        img{
            width: 100%;
            height: 100%;
            object-fit: cover;
            object-position: top;
        }
    }
</style>