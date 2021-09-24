<template>
    <header>
        <div id="nav_bar">

                <a class="logo" href="#">
                    <img src="../assets/images/dc-logo.png" alt="DC logo">
                </a>
            

                <ul class="menu">
                    <li><a href="#">Home</a></li>
                    <li><a href="#">Home</a></li>
                    <li><a href="#">Home</a></li>
                    <li><a href="#">Home</a></li>
                    <li><a href="#">Home</a></li>
                    <li><a href="#">Home</a></li>
                    <li><a href="#">Home</a></li>
                    <li><a href="#">Home</a></li>
                    <li><a href="#">Home</a></li>
                    
                </ul>
        </div>
    </header>
</template>

<script>
export default {
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";
@import "../style/style.css";

header{
    //Style
    background-color: $secondaryColor;
    font-family: $headerFont;
    //Spacing and Sizing
    padding-top: 110px;

    #nav_bar{
        background-color: #ffffff;
        height: 110px;
        //Flex Settings
        display: flex;
        justify-content: space-evenly;
        
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
            //Flex Settings
            display: flex;

            li{
                margin: 0 15px;
                transition: .3s ease-in-out;

                a{
                    //Style
                    text-decoration: none;
                    font-weight: 500;
                    //Spacing and Sizing
                    line-height: 110px;
                    transition: .3s ease-in-out;                    
                }

                &:hover{
                    border-bottom: 5px solid $primaryColor;
                    a{
                        color: $primaryColor;
                    }
                }
            } 
            
        }
    }
}
</style> 