<template>
    <div class="card_element"></div>
</template>

<script>
export default {
    
}
</script>

<style scoped>
.card_element{
    /* Style */
    background-color: indianred;
    border: 1px solid black;
    /* Spacing and Dimensions */
    height: 100px;
    margin: 5px;

    /* Flex Settings */
    flex-basis: calc(100% / 6 - 10px);
}
</style>