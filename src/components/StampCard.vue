<template>
    <div class="py-4">
        <img :src="img" :alt="`Immagine del fumetto ${titolo}`">
        <div class="">
            <h5 class="my-font-size">{{ titolo }}</h5>
        </div>
    </div>
</template>

<script>
    export default{
        name:"StampCard",
        props:{
            img: String,
            titolo: String,
        },
        data(){

        }
    }
</script>


<style scoped>
.my-font-size{
    font-size: 15px;
    color:white;
}

</style>