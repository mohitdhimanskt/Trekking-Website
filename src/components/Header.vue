<template>
  <div class="flex items-center justify-between flex-wrap bg-white-100 p-2">
    <div class="header">
      <router-link to="/">
        <img class="block h-16 sm:h-14 rounded-full mx-auto mb-4 sm:mb-0 sm:mr-4 sm:ml-0 " src="https://farout.herokuapp.com/static/FOH.PNG" />
      </router-link>
      <h5 class="flex item-right text-red-400 text-xs sm:text-sm md:text-base  lg:text-lg">Far Out Himalaya</h5>
      <div class="text-center px-4 py-2  mt-4 lg:mt-0">
        <router-link to="/about">
          <span class=" px-3 py-2  Black-text-teal-200 border-teal-400 hover:text-black hover:border-white ">ABOUT US</span>
        </router-link>
        <router-link to="/login">
          <span class="  px-3 py-2 border rounded blue-text-teal-400 border-teal-400 hover:text-black hover:border-white">LOGIN</span>
        </router-link>
        <router-link to="/Sign up">
          <span class="  px-3 py-2 border rounded blue-text-teal-400 border-teal-400 hover:text-black hover:border-white">SIGN UP</span>
        </router-link>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "Header",
  props: {
    title: String,
  },
  data: function () {
    return {
      name: "Mohit",
    };
  },
};
</script>




