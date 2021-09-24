<template>
    <footer>
        <div id="foooter_menu">  
            <div class="column">
                <div class="dc_comics_menu">
                    <h3>dc comics</h3>
                    <ul>
                        <li>
                            <a href="#">Characters</a>
                        </li>
                        <li>
                            <a href="#">Characters</a>
                        </li>
                        <li>
                            <a href="#">Characters</a>
                        </li>
                        <li>
                            <a href="#">Characters</a>
                        </li>
                        <li>
                            <a href="#">Characters</a>
                        </li>
                        <li>
                            <a href="#">Characters</a>
                        </li>
                        <li>
                            <a href="#">Characters</a>
                        </li>
                    </ul>
                </div>
                <div class="shop_menu">
                    <h3>shop</h3>
                    <ul>
                        <li>
                            <a href="">Shop DC</a>    
                        </li>
                        <li>
                            <a href="">Shop DC</a>    
                        </li>
                    </ul>
                </div>  
            </div>

            <div class="column">
                <div class="dc_menu">
                    <h3>dc</h3>
                    <ul>
                        <li>
                            <a href="#">Terms of Use</a>
                        </li>
                        <li>
                            <a href="#">Terms of Use</a>
                        </li>
                        <li>
                            <a href="#">Terms of Use</a>
                        </li>
                        <li>
                            <a href="#">Terms of Use</a>
                        </li>
                        <li>
                            <a href="#">Terms of Use</a>
                        </li>
                        <li>
                            <a href="#">Terms of Use</a>
                        </li>
                        <li>
                            <a href="#">Terms of Use</a>
                        </li>
                        <li>
                            <a href="#">Terms of Use</a>
                        </li>
                        <li>
                            <a href="#">Terms of Use</a>
                        </li>
                        <li>
                            <a href="#">Terms of Use</a>
                        </li>
                        <li>
                            <a href="#">Terms of Use</a>
                        </li>
                    </ul>
                </div>
            </div>

            <div class="column">
                <div class="sites_menu">
                    <h3>sites</h3>
                    <ul>
                        <li>
                            <a href="#">DC</a>
                        </li>
                        <li>
                            <a href="#">DC</a>
                        </li>
                        <li>
                            <a href="#">DC</a>
                        </li>
                        <li>
                            <a href="#">DC</a>
                        </li>
                        <li>
                            <a href="#">DC</a>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";
@import "../style/style.css";

footer{
    font-family: $primaryFont;
    //Background Images Settings
    background-image: url(../assets/images/dc-logo-bg.png), url(../assets/images/footer-bg.jpg);
    background-position: 70% 50%,  center;
    background-repeat: no-repeat;
    background-size: auto, cover;
    
    #foooter_menu{
        display: flex;
        height: 100%;
        padding: 30px 120px;
        
        .column{
            margin: 0 30px;

            h3{
                color: #ffff;
                text-transform: uppercase;
            }

            ul{
                list-style-type: none;

                a{
                    text-decoration: none;
                    color: grey;
                    font-size: .7rem;
                    transition: .3s ease-in-out;                    
                    
                    &:hover{
                        color: $primaryColor;
                    }
                }
            }
        }   
    }
}
</style>