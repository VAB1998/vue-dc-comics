<template>
    <div class="card_element">
        <img :src="imageSource" alt="series">
        <h4>{{series}}</h4>
    </div>
</template>

<script>
export default {
    name : 'Card',
    props : ['series', 'imageSource']
}
</script>

<style lang="scss" scoped>
.card_element{
    //Style
    color: #ffff;
    //Spacing and Dimensions 
    margin: 5px;

    //Flex Settings 
    flex-basis: calc(100% / 6 - 10px);

    img {
        width: 100%;
        height: 161px;
        object-fit: cover;
        object-position: top;
    }
}
</style>