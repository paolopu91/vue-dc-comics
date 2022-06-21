<template>
    <div class="bg-white my-nav-container">
        <div class="container d-flex align-items-center">

            <div class="container d-flex">

                <img src="/img/dc-logo.png" alt="Logo Dc">

            </div>   
                <ul class="nav flex-nowrap">
                    <li class="nav-item my-font-size" :key="i" v-for="(link,i) in navLinks">
                        <a class="nav-link active text-dark" aria-current="page" :href="link.href">
                        {{link.name}}
                        </a>
                    </li>
                </ul>
                
        </div>
    </div>    
</template>

<script>
    export default{
        name:"TheNavbar",
        data (){
            return{
                navLinks:[
                    {
                        name:"CHARACTERS",
                        href:"#"
                    },
                    {
                        name:"COMICS",
                        href:"#"
                    },
                    {
                        name:"MOVIE",
                        href:"#"
                    },
                    {
                        name:"TV",
                        href:"#"
                    },
                    {
                        name:"GAMES",
                        href:"#"
                    },
                    {
                        name:"COLLECTIBLES",
                        href:"#"
                    },
                    {
                        name:"VIDEOS",
                        href:"#"
                    },
                    {
                        name:"FANS",
                        href:"#"
                    },
                    {
                        name:"NEWS",
                        href:"#"
                    },
                    {
                        name:"SHOP",
                        href:"#"
                    },
                ]
            }
        }
    }
</script>



<style scoped>
    .my-nav-container{
        z-index: 999;
        position: relative;
        top: 15px;
    }
    .my-font-size{
        font-size: 15px;
    }
    .my-font-size:hover{
        border-bottom: 4px solid blue;
    }
</style>