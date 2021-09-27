<template>
    <footer>
        <div id="foooter_menu">  
            <div class="column">
                <div class="dc_comics_menu">
                    <h3>dc comics</h3>
                    <ul>
                        <li  v-for="(link, index) in dcComicslinks" :key="index">
                            <a :href="link.href">{{link.text}}</a>
                        </li>
                    </ul>
                </div>
                <div class="shop_menu">
                    <h3>shop</h3>
                    <ul>
                        <li  v-for="(link, index) in dcshoplinks" :key="index">
                            <a :href="link.href">{{link.text}}</a>
                        </li>
                    </ul>
                </div>  
            </div>

            <div class="column">
                <div class="dc_menu">
                    <h3>dc</h3>
                    <ul>
                        <li  v-for="(link, index) in dclinks" :key="index">
                            <a :href="link.href">{{link.text}}</a>
                        </li>
                    </ul>
                </div>
            </div>

            <div class="column">
                <div class="sites_menu">
                    <h3>sites</h3>
                    <ul>
                        <li  v-for="(link, index) in siteslinks" :key="index">
                            <a :href="link.href">{{link.text}}</a>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
        <div id="footer_bottom">

            <a :href="signuplink.href">{{signuplink.text}}</a>
            
            <div class="social_media_buttons">
                <h3>follow us</h3>
                <a v-for="(social, index) in socials" :key="index" :href="social.href">
                    <img :src="social.src" :alt="social.name">
                </a>
            </div>
        </div>
    </footer>
</template>

<script>
export default{
    name: 'Header',
    data: function(){
        return{
            dcComicslinks: [
                {
                    text: 'Characters',
                    href: '#characters',
                },
                {
                    text: 'Comics',
                    href: '#comics',
                },
                {
                    text: 'Movies',
                    href: '#movies',
                },
                {
                    text: 'TV',
                    href: '#tv',
                },
                {
                    text: 'Games',
                    href: '#games',
                },
                {
                    text: 'Videos',
                    href: '#videos',
                },
                {
                    text: 'News',
                    href: '#news',
                }
            ],

            dcshoplinks: [
                {
                    text: 'Shop DC',
                    href: '#shopdc',
                },
                {
                    text: 'Shop DC Collectibles',
                    href: '#shopdccollectibles',
                }
            ],

            dclinks: [
                {
                    text: 'Terms of use',
                    href: '#privacypolicy',
                },
                {
                    text: 'Ad Choices',
                    href: '#adchoices',
                },
                {
                    text: 'Advertising',
                    href: '#advertising',
                },
                {
                    text: 'Jobs',
                    href: '#jobs',
                },
                {
                    text: 'Substritions',
                    href: '#subscritions',
                },
                {
                    text: 'Talent Workshops',
                    href: '#talentworkshops',
                },
                {
                    text: 'CPSC Cerificates',
                    href: '#cpsccertificates',
                },
                {
                    text: 'Ratings',
                    href: '#ratings',
                },
                {
                    text: 'Shop Help',
                    href: '#shophelp',
                },
                {
                    text: 'Contact Us',
                    href: '#contactus',
                }
            ],

            siteslinks: [
                {
                    text: 'DC',
                    href: '#dc',
                },
                {
                    text: 'MAD Magazine',
                    href: '#madmagazine',
                },
                {
                    text: 'DC Kids',
                    href: '#dckids',
                },
                {
                    text: 'DC Universe',
                    href: '#dcuniverse',
                },
                {
                    text: 'DC Power Visa',
                    href: '#dcpowervisa',
                }
            ],

            signuplink: {
                text: 'sign-up now!',
                href: '#signup',
            },

            socials: [
                {
                    name: 'facebook',
                    href: '#facebook',
                    src : require('../assets/images/footer-facebook.png')
                },
                {
                    name: 'twitter',
                    href: '#twitter',
                    src : require('../assets/images/footer-twitter.png')
                },
                {
                    name: 'youtube',
                    href: '#youtube',
                    src : require('../assets/images/footer-youtube.png')
                },
                {
                    name: 'pinterest',
                    href: '#pinterest',
                    src : require('../assets/images/footer-pinterest.png')
                },
                {
                    name: 'periscope',
                    href: '#periscope',
                    src : require('../assets/images/footer-periscope.png')
                }
            ] 
        }          
    }
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";
@import "../style/general.scss";

footer{
    font-family: $primaryFont;
    
    #foooter_menu{
        //Spacing and Dimensions
        height: 100%;
        padding: 40px 120px;
         //Background Images Settings
        background-image: url(../assets/images/dc-logo-bg.png), url(../assets/images/footer-bg.jpg);
        background-position: 70% 50%,  center top;
        background-repeat: no-repeat;
        background-size: auto, cover;
        //Flex Settings
        display: flex;

        .column{
            margin-right: 30px;

            h3{
                //Style
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

    #footer_bottom{
        //Style
        background-color: #303030;
        //Spacing and Dimensions
        height: 100px;
        padding: 0 120px;
        //Flex Settings
        display: flex;
        justify-content: space-between;
        align-items: center;

        >a{
            //Style
            color: #ffffff;
            text-decoration: none;
            text-transform: uppercase;
            border: 2px solid $primaryColor;
            //Sizing and Dimensions
            padding: 8px;
            //Other Settings
            transition: .3s ease-in-out;                    

            &:hover{
                background-color: $primaryColor;
            }    
        }
        .social_media_buttons{
            //Flex Settings
            display: flex;
            align-items: center;
            justify-content: space-between;

            h3{
                //Style
                color: $primaryColor;
                text-transform: uppercase;
                //Spacing and Dimensions
                margin-right: 15px;
            }
            a{
                //Spacing and Dimensions
                margin-right: 15px;
                //Other Settings
                transition: .3s ease-in-out;  

                &:hover{
                    opacity: .8;
                }
            }
        }
    }
}
</style>