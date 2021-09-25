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
export default{
    name: 'Header',
    data: function(){
        return{

            links: [
                {
                    text: 'characters',
                    url: '#characters',
                    current: false
                },
                {
                    text: 'comics',
                    url: '#comics',
                    current: true
                },
                {
                    text: 'movies',
                    url: '#movies',
                    current: false
                },
                {
                    text: 'tv',
                    url: '#tv',
                    current: false
                },
                {
                    text: 'games',
                    url: '#games',
                    current: false
                },
                {
                    text: 'collectibles',
                    url: '#collectibles',
                    current: false
                },
                {
                    text: 'videos',
                    url: '#videos',
                    current: false
                },
                {
                    text: 'fans',
                    url: '#fans',
                    current: false
                },
                {
                    text: 'news',
                    url: '#news',
                    current: false
                },
                {
                    text: 'shop',
                    url: '#shop',
                    current: false
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";
@import "../style/style.css";

header{
    //Style
    font-family: $primaryFont;
    padding: 0 120px;

    #nav_bar{
        //Style
        background-color: #ffffff;
        //Spacing and Dimensions
        height: 110px;
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
}
</style> 