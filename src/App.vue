<template>
  <div class="body">

    <TheNavbar />


    <main>
      <div class="container padding-top">
        <h1 class="text-light fs-6 text "> --> CONTENT GOES HERE -- </h1>
      </div>
    </main>
    <TheFooter />

    <BannerSignUp />

  </div>
</template>

<script>

import TheFooter from './components/TheFooter.vue'
import TheNavbar from './components/TheNavbar.vue'
import BannerSignUp from './components/BannerSignUp.vue'

export default {
  name: 'App',
  components: {
    TheFooter,
    TheNavbar,
    BannerSignUp
}
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.body{
  background-color: black;
}
.padding-top{
  padding-top: 4rem;
}
</style>
