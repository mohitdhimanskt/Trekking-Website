<template>
  <div class="flex flex-col mx-4 items-center bg-white-200 px-4 py-40 rounded-tb rounded-lr border-solid border-4 border-gray-400">
    <h2 class=" block text-pink-400 mx-2 text-center text-4xl font-serif m-0 font-medium leading-none py-2">{{$route.params.services}}</h2>
    <p class="block italic text-gray-600 text-center font-serif m-0 p-4 font-medium leading-none text-xl ">
  {{content}}
    </p>
  </div>
</template>
<script>
export default {
  data: function() {
    return{
      content: ''
    }
  },
  mounted(){
    this.getApiData()
  },
  methods: {
    getApiData(){
     fetch('https://fakerapi.it/api/v1/texts?_quantity=1&_characters=500')
        .then(response => response.json())
        .then(data => {
          this.content = data.data[0].content;
        }).catch(err => console.log(err))
    }
  }
}
</script>

