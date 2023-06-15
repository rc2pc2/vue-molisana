<script >
import MainNavbar from './components/MainNavbar.vue'

export default {
    name: 'App',
    components:{
      MainNavbar
    }
}
</script>

<template>
  <h1>
    App H1
  </h1>
  <MainNavbar />

</template>

<style>
/* importare i file css da condividere con tutto il progetto */

  h1{
    color: blue;
  }
</style>
