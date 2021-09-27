<template>
    <main>
        <section id="cards">
            <Card />
        </section>
    </main>
</template>

<script>
import Card from './Card.vue'

export default {
    name : 'Main',
    components : {
        Card
    },

    data : function(){
        return{

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
    // Spacing and Dimensions
    padding: 0 120px;

    #cards{
        //Flex Settings
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    }
    
}
</style> 