<template>
  <div class="section">
    <div>
      <h2 class="text-center text-red-600 text-xs sm:text-sm md:text-base xl:text-xl">What we do?</h2>
      <p class="mt-2 text-lg text-gray-600">
        Quickly build an effective pricing table for your potential customers<br>
        with this layout. It's built with default Material-UI components with<br>
        little customization.
      </p>
    </div>
    <div class="recent-item">
       <router-link  v-for="item in servicesArr" :key="item.name"  :to="item.path">
        <button class="recent-item " type="button"  v-bind:style='{ backgroundImage: "url(" + item.url + ")", }'>
          <span class="recent-item">{{item.name}}</span>
        </button>
     </router-link> 
    </div>
  </div>
</template>
<script>    
export default {
  name: "Services",
  data: function () {
    return {
      servicesArr: [
        {
           name: "Skiing",
           url: 'https://img3.oastatic.com/img2/40917734/600x300r/rehjan-latu-ura-9-km-kajaani-finland.jpg',
          path: 'skiing'
        },

        {
          name: "Trekking (backpacking)",
          url: "https://di-uploads-pod5.dealerinspire.com/triplejsaipan/uploads/2019/03/Three-People-Hiking-Up-Mountain_24359265.jpg",
          path: 'trekking'
          
        },
        {
          name: "Mountain Biking",
          url: "https://bikefeatures.com/wp-content/uploads/2018/07/Best-Mountain-Bikes-Under-1000.jpg",
          path:'moutainbiking'
        },
        {
          name: "Local Sight Seeing",
          url: "https://assets.traveltriangle.com/blog/wp-content/uploads/2016/02/manali-river-beas.jpg",
          path: 'localsightseeing'
        },
        {
          name: "Jeep Safari",
          url: "https://www.picnicwale.com/assets/adventure/manali-jeep-safari-season.jpg",
          path: 'jeepsafari'
        },
        {
          name: "Expedition Climbing",
          url: "https://www.alpineinstitute.com/media/274036/denali_expedition_climbing_summit_ridge.jpg",
          path: 'expeditionclimbing'
        },
        {
          name: "Family Trips",
          url: "https://i.pinimg.com/736x/24/61/03/246103a96862eeab2dc50a74a7de8cac.jpg",
          path: 'familytrips'
        },
        {
          name: "Day Hikes",
          url: "https://img.traveltriangle.com/blog/wp-content/uploads/2019/04/Trekking-In-Himachal-Pradesh-cover.jpg",
          path: 'dayhikes'
        },
        {
          name: "Canyoning",
          url: "https://bluberryholidays.com/wp-content/uploads/2020/05/a8apdxyy5wmrddt.jpg",
          path: 'canyoning'
        },
        {
          name: "Cycling",
          url: "https://www.bbcgoodfood.com/sites/default/files/editor_files/2020/05/cycling_3.jpg",
          path: 'cycling'
        },
      ],
     };
  },
};
</script>
<style scoped>
/* h2 {
  color: #f5004c;
  text-align: center;
  margin-bottom: 0.35em;
  font-size: 3.75rem;
  font-family: "Roboto", "Helvetica", "Arial", sans-serif;
  font-weight: 300;
  line-height: 1;
  letter-spacing: -0.00833em;
} */
/* P {
  color: rgba(0, 0, 0, 0.54);
  text-align: center;
  font-size: 1.25rem;
  font-family: "Roboto", "Helvetica", "Arial", sans-serif;
  font-weight: 500;
  margin: 0;
  display: block;
  line-height: 1.6;
  letter-spacing: 0.0075em;
  margin-bottom: 16px;
} */

.recent-item {
  width: 30%;
  height: 300px;
  position: relative;

  color:black;
  border: 0;
  margin: 0;
  cursor: pointer;
  display: initial;
  outline: none;
  padding: 0;
/* 
  align-items: center;
  user-select: none;
  border-radius: 0;
  vertical-align: middle;
  justify-content: center;

  text-decoration: none;

  -webkit-tap-highlight-color: transparent; */
}
</style>