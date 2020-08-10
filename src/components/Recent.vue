<template>
<div>
<div class ="recent">
<h4 class="text-center text-red-600 text-xs sm:text-sm md:text-base  lg:text-lg">Featured Treks</h4>
<p class="mt-2 text-lg text-gray-600">Quickly build an effective pricing table for your potential customers<br>
    with this layout. It's built with default Material-UI components with<br> 
                       little customization.</P>
</div>
<div class ="recent-item">
    <router-link to="/button">  <span class="item-trek">4 Days hiking programme</span>
    <span class="item-trek">06 November 2018</span></router-link>
    
    </div>
    <div class="hiking">
        <P> 4 Days hiking programme </p>
      <router-link to="/button"> <button class="recent" type="button"><span class="recent">LEARN MORE</span></button></router-link>
    </div>
<div class="item">
    <router-link to="/button">  <span class="trek">Hamta Circle trek</span>
    <span class="trek">06 November 2018</span></router-link>
</div>

<div class="hiking1">
    <p> Hamta Circle Trek </P>
    <router-link to="/button"><button class="recent" type="button"><span class="recent">LEARN MORE </span></button></router-link>
</div>
<router-link to="/button"><button class="bg-purple-500 hover:bg-blue-600 text-black font-bold py-2 px-4 rounded" type="button"><span class="recent">SHOW MORE </span></button></router-link>
</div>
</template>
<script>

export default {
    name: 'Recent',
    props: {
        // name: String
    },
    data: function() {
        return{
        // name: 'treks'
        }
    }

}
</script>
<style scoped>

 .recent-item{
     height: 100%;
     display: flex;
     max-width: 400px;
     flex-direction: column;
     overflow: hidden;
    box-shadow: 0px 1px 3px 0px rgba(0, 0, 0, 0.2), 0px 1px 1px 0px rgba(0, 0, 0, 0.14), 0px 2px 1px -1px rgba(0, 0, 0, 0.12);
    border-radius: 4px;
    background-color: #fff;
 }
 .item{
       height: 100%;
     display: flex;
     max-width: 400px;
     flex-direction: column;
     overflow: hidden;
    box-shadow: 0px 1px 3px 0px rgba(0, 0, 0, 0.2), 0px 1px 1px 0px rgba(0, 0, 0, 0.14), 0px 2px 1px -1px rgba(0, 0, 0, 0.12);
    border-radius: 4px;
    background-color: #fff;
 }
 .hiking{
        height: 100%;
     display: flex;
     max-width: 400px;
     flex-direction: column;
     overflow: hidden;
    box-shadow: 0px 1px 3px 0px rgba(0, 0, 0, 0.2), 0px 1px 1px 0px rgba(0, 0, 0, 0.14), 0px 2px 1px -1px rgba(0, 0, 0, 0.12);
    border-radius: 4px;
    background-color: #fff;
 }
 .hiking1{
        height: 100%;
     display: flex;
     max-width: 400px;
     flex-direction: column;
     overflow: hidden;
    box-shadow: 0px 1px 3px 0px rgba(0, 0, 0, 0.2), 0px 1px 1px 0px rgba(0, 0, 0, 0.14), 0px 2px 1px -1px rgba(0, 0, 0, 0.12);
    border-radius: 4px;
    background-color: #fff;
 }
 </style>