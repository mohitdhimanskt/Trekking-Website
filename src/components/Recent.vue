<template>
<div>
<div class ="recent">
<h4 class="text-center text-red-600 text-xs sm:text-sm md:text-base  lg:text-lg">Featured Treks</h4>
<p class="mt-2 text-lg text-gray-600">Quickly build an effective pricing table for your potential customers<br>
    with this layout. It's built with default Material-UI components with<br> 
                       little customization.</P>
</div>
<div class="flex flex-col mx-4 items-center bg-white-200 px-4 py-40 rounded-tb rounded-lr border-solid border-4 border-gray-400">
<div class="flex flex-col bg-white sm h-20 text-left overflow-hidden  ">
    <router-link to="/button">  <span class="item-trek">4 Days hiking programme</span>
    <span class="item-trek">06 November 2018</span></router-link>
    
    </div>
    <div class="flex flex-col bg-white sm h-full text-left overflow-hidden">
        <P> 4 Days hiking programme </p>
      <router-link to="/button"> <button class="recent" type="button"><span class="recent">LEARN MORE</span></button></router-link>
    </div>
<div class="flex flex-col bg-white sm h-20 overflow-hidden mx-8 my-2">
    <router-link to="/button">  <span class="trek">Hamta Circle trek</span>
    <span class="trek">06 November 2018</span></router-link>
</div>

<div class="flex flex-col bg-white sm h-full overflow-hidden  text-right mx-4">
    <p> Hamta Circle Trek </P>
    <router-link to="/button"><button class="recent" type="button"><span class="recent">LEARN MORE </span></button></router-link>
</div>
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
