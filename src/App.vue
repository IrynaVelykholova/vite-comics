<script>
  import TheHeader from "./components/TheHeader.vue"
  import TheFooter from "./components/TheFooter.vue"

  export default {
    components:{
      TheHeader,
      TheFooter,
    }
} 
</script>

<template> 
  <TheHeader></TheHeader>
  <main> Content goes here</main>
  <ThePreFooter></ThePreFooter>
  <TheFooter></TheFooter>
</template>
<style>  </style>

