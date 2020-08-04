<template>
  <div class="home">
    <Heroslider></Heroslider> 
    <Services></Services>
    <Recent></Recent>

    
  </div>
</template>

<script>

import Heroslider from "@/components/Heroslider.vue";
import Services from "@/components/Services.vue";
import Recent from "@/components/Recent.vue";

  
export default {
  name: "Home",
  components: {
    Heroslider,
    Services,
    Recent,

  
  },
};
</script>
