<template>
  <TheNFT />
</template>

<script>
import TheNFT from "@/components/TheNFT.vue"

export default {
  name: 'App',
  components: {
    TheNFT
  }
}
</script>

<style>
@import url("https://fonts.google.com/specimen/Outfit");
#app {
  font-family: "Outfit", sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
body{
  background-color: hsl(217, 54%, 11%);
}

</style>
