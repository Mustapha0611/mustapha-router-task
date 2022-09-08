<template>

<div class="main">
      <div class="sub_main">
        <h2 >Hi, I'm Mustapha</h2>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. 
          Delectus perferendis consequatur repudiandae odio sunt eos 
          animi dolorum, commodi repellendus iste, velit at maiores! Illum, 
          ipsa tempore dolores ducimus quos porro.
        </p>
        <button id="btn">Lorem ipsum</button>
      </div>
    </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.main{
  /* background:url(assets/279547.jpg) #004; */
  background-color: #2c3e50;
  background-size: cover;
  display:flex;
  justify-content: center;
  align-items:center;
  height:90vh;
  padding:5px 5%;
}
.sub_main >h2{
  font-size:4em;
}
.sub_main > p{
  width:50%;
  margin:10px 0;
}
#btn{
  border:3px solid rgb(199, 199, 199);
  border-radius:7px;
  background: transparent;
  color:#fff;
  padding:5px 15px;
}

#btn:hover{
  background:#dbdbdb;
  transition:.2s;
  color:rgb(12, 11, 11);
}
</style>
