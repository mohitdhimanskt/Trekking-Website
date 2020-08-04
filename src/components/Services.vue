<template>
      <div class="section">
      <div>
            <h2>What we do?</h2>
            <p>
                Quickly build an effective pricing table for your potential customers
                 with this layout. It's built with default Material-UI components with 
                                   little customization.
            </p>
            
        </div>
        <div class="recent-item">
            <button class="recent-item" type="button" v-for="item in servicesArr" :key="item">
                <span class="recent-tem">{{item}}</span>
            </button>

        </div>
    </div>
</template>
<script>
export default {
    name: 'Services',
    data: function () {
        return {
            servicesArr: [  
       
               "Skiing",
            
               "Trekking (backpacking)",
           
               "Mountain Biking",
           
               "Local Sight Seeing",
           
               "Jeep Safari",
            
               "Expedition Climbing",
           
               "Family Trips",
           
               "Daily Hikes",
            
               "Canyoning",
           
               "Cyling"
           ]
        }
    }
}

</script>
<style scoped>
h2{
    color: #f5004c;
    text-align: center;
    margin-bottom: 0.35em;
    font-size: 3.75rem;
    font-family: "Roboto", "Helvetica", "Arial", sans-serif;
    font-weight: 300;
    line-height: 1;
    letter-spacing: -0.00833em;
}
P{
    color:  rgba(0, 0, 0, 0.54);
    text-align: center;
        font-size: 1.25rem;
    font-family: "Roboto", "Helvetica", "Arial", sans-serif;
    font-weight: 500;
    margin: 0;
    display: block;
    line-height: 1.6;
    letter-spacing: 0.0075em;
}
.recent-item{
    width: 30%;
    height: 300px;
    position: relative;
    
    color: inherit;
    border: 0;
    margin: 0;
    cursor: pointer;
     display: initial; 
    outline: none;
     padding: 0; 
    
     align-items: center; 
     user-select: none; 
     border-radius: 0; 
     vertical-align: middle; 
     justify-content: center; 

     text-decoration: none; 
    
     
    -webkit-tap-highlight-color: transparent; 
}
</style>