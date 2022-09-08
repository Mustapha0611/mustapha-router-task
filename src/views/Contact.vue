<template>
  <div class="contact">
      <form action="">
        <h2>Contact Form</h2>
        <input type="text" placeholder="Enter your Name here..." required v-model="Name">
        <input type="email" placeholder="Enter your Email here..." required v-model="mail">
        <input type="text" placeholder="Enter your Number here..." required v-model="number">
        <textarea name="" id="" cols="30" rows="10" placeholder="Type A message " v-model="message"></textarea>
        <button type="submit" @click.prevent="handleSubmission">Send A Message</button>
       </form> 
       <div class="Modal" v-if="isFilled">
          <p>Name:{{Name}}</p>
          <p>Email: {{mail}}</p>
          <p>Number: {{number}}</p>
          <p>Message: {{message}}</p>
          <button @click="handleClose">Close</button>
       </div>
  </div>
 
</template>

<script>   
export default {
  data(){
    return{
      Name:'',
      mail:'',
      number:'',
      message:'',
      isFilled:false
    } 
  },
  methods:{
    handleSubmission(){
      this.isFilled = true
    },
    handleClose(){
      this.isFilled = false
      this.Name = ''
      this.mail = ''
      this.number = ''
      this.message = ''
    }
  }
}
</script>

<style scoped>
  .contact{
    background: url('../assets/279547.jpg');
  background-size: cover;
  display:flex;
  /* justify-content: center; */
  align-items:center;
  height:90vh;
  padding:5px 5%;
  }
  form{
    display:flex;
    flex-direction: column;
  }
  input[type="text"], input[type="email"] ,textarea{
    margin:10px 0;
    width:150%;
    border:none;
    border-radius: 7px;
    padding:10px ;
  }
  button{
    border:none;
    padding :10px;
    width:50%;
    border-radius:5px;
  }
  .Modal{
    width:30%;
    position:absolute;
    background: #fff;
    min-height:35vh;
    margin:10px 35%;
    border-radius:7px
  }
  .Modal > p{
    color : black;
    margin:10px 5%;
  }
  .Modal > button{
    position:absolute;
    width:40%;
    color: #fff;
    background:rgb(44, 44, 252);
    margin:5px 30%;
    border-radius:5px;
    bottom:10px;
  }
</style>