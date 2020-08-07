<template>
  <div class="service">
    <h2>{{$route.params.services}}</h2>
    <p>
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
<style scoped>
.service{
height: calc(100% - 64px);
    display: flex;
    padding: 16px 24px 24px;
    margin-top: 8px;
    align-items: center;
    flex-direction: column;
    box-shadow: 0px 1px 5px 0px rgba(0, 0, 0, 0.2), 0px 2px 2px 0px rgba(0, 0, 0, 0.14), 0px 3px 1px -2px rgba(0, 0, 0, 0.12);
   border-radius: 4px;
       background-color: #fff;
}
h2{
  color: #F5004c;
  margin-bottom: 0.35em;
  text-align: center;
  font-size: 3.75rem;
    font-family: "Roboto", "Helvetica", "Arial", sans-serif;
    font-weight: 300;
    line-height: 1;
    letter-spacing: -0.00833em;
    margin: 0px;
    display: block;
}
p{
      color: rgba(0, 0, 0, 0.54);
      text-align: center;
          font-size: 1.25rem;
    font-family: "Roboto", "Helvetica", "Arial", sans-serif;
    font-weight: 500;
    line-height: 1.6;
    letter-spacing: 0.0075em;
    margin: 0;
    display: block;
    padding: 65px;
}
</style>