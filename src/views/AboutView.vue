<template>
  <div class="about">
    <h2>About US</h2>
   <div>
      <ul class="services">
        <li v-for="service in Services" :key="service.title">
          <img :src="service.logo">
          <h3>{{ service.title }}</h3>
          <p>{{ service.para }}</p>
        </li>
      </ul>
   </div>
  </div>
</template>
<script>
export default {
  data(){
    return{
      Services:[
        {logo:require('../assets/phone.png'), title:'Mobile Friendly', para:'Sed vel vulputate lacus. Nulla et fringilla turpis. Etiam non urna magna. Fusce rutrum nec eros id dapibus. In tincidunt mi eget molestie condimentum'},
        {logo:require('../assets/anemone.png'), title:'EASY-TO-USE', para:'Sed vel vulputate lacus. Nulla et fringilla turpis. Etiam non urna magna. Fusce rutrum nec eros id dapibus. In tincidunt mi eget molestie condimentum'},
        {logo:require('../assets/clear.png'), title:'FREE', para:'Sed vel vulputate lacus. Nulla et fringilla turpis. Etiam non urna magna. Fusce rutrum nec eros id dapibus. In tincidunt mi eget molestie condimentum'}
      ]
    }
  }
}
</script>
<style scoped>
.about{
 background:rgb(230, 225, 225);
  background-size: cover;
  display:flex;
  justify-content: center;
  align-items:center;
  height:90vh;
  padding:5px 5%;
}
h2{
  position:absolute;
  top:70px;
  color:black

}
.services{
  display:flex;
  

}
.services > li{
  list-style:none;
  margin:20px 2%;
  width:30%;
  height:70vh;
  text-align:center;
  /* background:rgb(110, 110, 110);  */
  padding:5px 10px;
  border-radius:10px;
  color:black
}
</style>