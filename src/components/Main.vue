<template>
    <main>
        <section id="cards">
            <Card v-for="(card, index) in DataCards" 
            :key="index" :series="card.series" :imageSource="card.thumb"/>
        </section>
    </main>
</template>

<script>
import Card from './Card.vue'
import DataCards from '../data/dataCards.js'
export default {
    name : 'Main',
    components : {
        Card
    },

    data : function(){
        return{
            DataCards
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";
@import "../style/general.scss";

main{
    // Style
    background-color: $secondaryColor;

    #cards{
        // Spacing and Dimensions
        padding: 20px 120px;
        //Flex Settings
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
    }
    
}
</style> 