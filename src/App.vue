<template>
  
  
  <HeaderComponente />

  <main class="content"><router-view /></main>

  
  <FooterComponente/>


</template>


<script>
import HeaderComponente from './components/HeaderComponente.vue';
import FooterComponente from './components/FooterComponente.vue';


export default {

components:{
HeaderComponente,
FooterComponente

},
data() {
return {
};
},
}


</script>

<style scoped>
  @import 'bootstrap/dist/css/bootstrap.min.css';  


body {
background-color: red;
}

h1 {
color: #D42401;
font-size: 28px
}
</style>
