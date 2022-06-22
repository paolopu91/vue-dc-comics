<template>
    <div class="card">
        <img :src="img" :alt="`Immagine del fumetto ${titolo}`">
        <div class="card-body">
            <h5>{{ titolo }}</h5>
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


<style>
</style>