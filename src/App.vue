<template>
  <div class="body">

    <TheNavbar />


    <main>
      <TheCardDc />
    </main>
    
    <TheFooter />

    <BannerSignUp />

  </div>
</template>

<script>

import TheFooter from './components/TheFooter.vue'
import TheNavbar from './components/TheNavbar.vue'
import BannerSignUp from './components/BannerSignUp.vue'
import TheCardDc from './components/TheCardDc.vue'

export default {
  name: 'App',
  components: {
    TheFooter,
    TheNavbar,
    BannerSignUp,
    TheCardDc
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
