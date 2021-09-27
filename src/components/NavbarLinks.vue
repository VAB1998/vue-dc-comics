<template>           
            <li  :class="{active : currentPage}">
                <a :href="anchorTag">{{text}}</a>
            </li> 
</template>

<script>

export default {
    props : {
        text : String,
        anchorTag : String,
        currentPage : Boolean
    },

    data : function (){
        return{
            
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";
@import "../style/general.scss";
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
</style>