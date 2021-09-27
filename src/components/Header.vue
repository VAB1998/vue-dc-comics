<template>
    <header>
        <Navbar />
        <Jumbotron />
    </header>
</template>

<script>
import Navbar from './Navbar.vue'
import Jumbotron from './Jumbotron.vue'
export default{
    name: 'Header',
    components : {
        Navbar,
        Jumbotron
    },

    data: function(){
        return{
            
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";
@import "../style/general.scss";

header{
    //Style
    font-family: $primaryFont;

}
</style> 