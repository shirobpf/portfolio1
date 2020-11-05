<template>
 <div>
  <Header />
  <Navi />
  <div class="main">
     <LeftMenu />
     <Productslist />
  </div>
  <Footer />  
 </div>
</template>
<script>
import Header from "../components/Header";
import LeftMenu from "../components/LeftMenu";
import Footer from "../components/Footer";
import Productslist from "../components/Productslist";
import Navi from "../components/Navi";
export default{
  components:{
    Header,
    Navi,
    LeftMenu,
    Productslist,
    Footer
  }
};

</script>
<style scoped>
.main{
  display: flex;
  margin: 10px 0;
}
</style>
