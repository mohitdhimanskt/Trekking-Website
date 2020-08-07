<template>
  <div id="footer">
    <div class="links">
      <h5>Far Out Himalayas</h5>
      <h5>1235 University Boulevard</h5>
      <h5>Steubenville, Ohio</h5>
      <h5>43952</h5>
      <h5>(740)283-3771</h5>
    </div>
    <div class="links5">
      <a href="https://www.linkedin.com" target="_blank">
        <i class="fa fa-linkedin-square" aria-hidden="true"></i>
      </a>
      <a href="https://www.twitter.com" target="_blank">
        <i class="fa fa-twitter" aria-hidden="true"></i>
      </a>
      <a href="https://www.youtube.com" target="_blank">
        <i class="fa fa-youtube" aria-hidden="true"></i>
      </a>
      
    </div>
    <div class="links6">
      <ul>
        <li>About Us</li>
        <li>Contact Us</li>
        <li>Gallery</li>
        <li>Privacy Policy</li>
        <li>Frequently Asked Question</li>
      </ul>
    </div>
  </div>
</template>
<script>
export default {
  name: "Footer",
  // props:{

  // }
};
// data: function() {
//  return{

//  }
</script>
<style scoped>
h5 {
  width: 100%;
  display: flex;
  flex-wrap: wrap;
  box-sizing: border-box;
}
li {
  list-style-type: none;
  color: #fff;
}
.links6 {
  text-align: end;
  margin-right: 70px;
  margin-top: -141px;
}
.links {
  background-color: dimgray;
  color: #fff;
}
</style>