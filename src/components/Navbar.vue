<template>
    <div id="nav_bar">

        <a class="logo" href="#">
            <img src="../assets/images/dc-logo.png" alt="DC logo">
        </a>

        <ul class="menu">

            <Menulinks v-for="(link, index) in links" :key="index" 
            :currentPage="link.current" :text="link.text" :anchorTag="link.url" />

        </ul>
    </div>
</template>

<script>
import Menulinks from './NavbarLinks.vue'
import links from '../data/navbarLinks.js'
export default {
    name: 'Navbar',
    components : {
        Menulinks
    },

    data : function (){
        return{
            links
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";
@import "../style/general.scss";

#nav_bar{
    //Style
    background-color: #ffffff;
    //Spacing and Dimensions
    height: 110px;
    padding: 0 120px;

    //Flex Settings
    display: flex;
    justify-content: space-between;
    
    .logo{
        align-self: center;

        img{
            //Spacing and Sizing
            width: 70px;
        }
    }

    .menu{
        //Style
        list-style-type: none;
        text-transform: uppercase;
        //Flex Settings
        display: flex;

        
    }
}
</style>