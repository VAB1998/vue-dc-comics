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

//Reset
*{
    padding: 0;
    margin: 0;
    box-sizing: border-box;
}

#nav_bar{
    // background-color: #ffffff;
    font-family: $headerFont;
    background-color: blue;
    height: 110px;
    //Flex Settings
    display: flex;
    justify-content: space-evenly;
    
    .logo{
        align-self: center;

        img{
            width: 70px;
        }
    }

    
    .menu{
        list-style-type: none;

        //Flex Settings
        display: flex;
        li{
            cursor: pointer;
            
            a{
            text-decoration: none;
            padding: 0 20px;
            line-height: 110px;
        
            }
        } 
        
    }
}
</style> 