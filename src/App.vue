<script>
//import del componente
import Header from './components/Header.vue';
import Footer from './components/Footer.vue';
import Main from './components/Main.vue';

//definizione del componente
export default {
  components: {
    Header,
    Footer,
    Main
  }

}
</script>


<template>
  
  <!-- stampo in pagina -->
  <Header />
  <Main />
  <Footer />
 
</template>


<style lang="scss">
// regole comuni a tutto (posso fare una cartella a parte anche, dentro assets, file .scss)
// @import url("google font");

*{
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

img{
  max-width: 100%;
}

ul {
  list-style-type: none;

  li{
    margin: 0 0.5rem;

    a{
      color: inherit;
      text-decoration: none;
    }
  }
}

</style>
