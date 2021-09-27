<template>
    <div id="nav_bar">

        <a class="logo" href="#">
            <img src="../assets/images/dc-logo.png" alt="DC logo">
        </a>

        <ul class="menu">

            <li :class="{active : link.current}" v-for="(link, index) in links" :key="index">
                <a :href="link.url">{{link.text}}</a>
            </li> 

        </ul>
    </div>
</template>

<script>
import links from '../data/navbarLinks.js'
export default {
    name: 'Navbar',


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

        li{
            margin: 0 15px;
            transition: .3s ease-in-out;

            a{
                //Style
                text-decoration: none;
                font-weight: 500;
                color: $secondaryColor;
                //Spacing and Sizing
                line-height: 110px;
                transition: .3s ease-in-out;                    
            }

            &:hover{
                border-bottom: 4px solid $primaryColor;
                a{
                    color: $primaryColor;
                }
            }
            &.active{
                border-bottom: 4px solid $primaryColor;
                a{
                    color: $primaryColor;
                }
            }
        } 
    }
}
</style>