<template>
    <footer>
        <div class="container">
            <div class="row">
                <div class="col d-flex pt-5 mt-2 my-font-size">
                    <div class="col">
                            <h2 class="text-light fs-4 text">
                                DC COMICS
                            </h2>
                            <ul class="list-unstyled text-white-50">
                                <li :key="i" v-for="(link,i) in linkFooterComics"> {{link}} </li>
                            </ul>
                            <h2 class="text-light fs-4 text">
                                SHOP
                            </h2>
                            <ul class="list-unstyled text-white-50">
                                <li :key="i" v-for="(element,i) in linkFooterShop"> {{element}} </li>
                            </ul>
                    </div>
                    <div class="col">
                            <h2 class="text-light fs-4 text">
                                DC
                            </h2>
                            <ul class="list-unstyled text-white-50">
                                <li :key="i" v-for="(item,i) in linkFooterDc">{{item}}</li>
                            </ul>
                    </div>
                    <div class="col">
                            <h2 class="text-light fs-4 text">
                                SITES
                            </h2>
                            <ul class="list-unstyled text-white-50">
                                <li :key="i" v-for="(unit,i) in linkFooterSite">{{unit}}</li>
                            </ul>
                    </div>
                </div>
                <div class="col">
                    <img src="/img/dc-logo-bg.png" alt="">
                </div>
            
            </div>
        </div>
    </footer>
</template>

<script>
    export default{
        name:"TheNavbar",
        data (){
            return{
                linkFooterComics:["Characters", "Comics", "Movies", "TV", "Games", "Videos", "News",],
                linkFooterShop:["Shop DC", "Shop DC Collectibles",],
                linkFooterDc:["Termo of Use", "Privacy Policy (New)", "Ad choice", "Advertising", "Jobs", "Subscriptions", "Talent Workshop", "CPSC Certificate", "Ratings", "Shop Help", "Contact US",],
                linkFooterSite:["DC", "Mad Magazin", "DC Kids", "DC Universe", "DC Power Visa",]
            }
            
        }
    }
</script>



<style scoped>
footer{
    background-image: url("/public/img/footer-bg.jpg");
}
.my-font-size{
    font-size: 15px;
}

</style>