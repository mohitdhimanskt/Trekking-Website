<template>
  <div class="service">
    <h2>{{$route.params.services}}</h2>
    <p>
      Quickly build an effective pricing table for your potential customers<br>
       with this layout. It's built with default Material-UI components with<br> 
                       little customization.
    </p>
  </div>
</template>
<script>
export default {
  mounted(){
    console.log(this.$route)
  }
}
</script>