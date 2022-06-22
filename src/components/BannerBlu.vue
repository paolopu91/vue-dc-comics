<template>
    <div class="bg-primary">
        <div class="container d-flex my-container">
            <div class="container d-flex " v-for="(element,i) in listImg" :key="i">
                
                <img class="my-img" :src="element.img" alt="Loghi DC">
                    
            </div>
        </div>
    </div>
</template>

<script>
export default{
    name:"BannedBlu",
    data (){
        return{
            listImg:[
                {
                    text: "DIGITAL COMICS",
                    img: "/img/buy-comics-digital-comics.png",
                },
                {
                    text: "DC MERCHANDAISER",
                    img: "/img/buy-comics-merchandise.png",
                },
                {
                    text: "SUBSCRIPTION",
                    img: "/img/buy-comics-subscriptions.png",
                },
                {
                    text: "COMIC SHOP LOCATOR",
                    img: "/img/buy-comics-shop-locator.png",
                },
                {
                    text: "DC POWER VISA",
                    img: "/img/buy-dc-power-visa.svg",
                },
            ]
        }
    }
}
</script>


<style scoped>
.my-container{
    padding: 1rem;
}
.my-img{
    width: 80px;
    height: 80px;
}
</style>