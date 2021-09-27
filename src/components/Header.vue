<template>
    <header>
        <Navbar />
    </header>
</template>

<script>
import Navbar from './Navbar.vue'

export default{
    name: 'Header',
    components : {
        Navbar
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
    padding: 0 120px;

}
</style> 