<template>
  <div class="home">
    <Heroslider></Heroslider> 
    <Services></Services>
    <Recent></Recent>
    <Footer></Footer>
    
  </div>
</template>

<script>

import Heroslider from "@/components/Heroslider.vue";
import Services from "@/components/Services.vue";
import Recent from "@/components/Recent.vue";
import Footer from "@/components/Footer.vue";
  
export default {
  name: "Home",
  components: {
    Heroslider,
    Services,
    Recent,
    Footer,
  
  },
};
</script>
