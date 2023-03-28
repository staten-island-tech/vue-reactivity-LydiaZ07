<template>
  <div class="home">
    <!-- <h1 :class="titleClass">{{ message }}</h1>
    <ul>
      <li v-for="animal in animals" :key="animal">{{ animal }}</li>
    </ul>
    <button @click="authState" v-if="loggedIn">Log Out</button>    @ = src, quicker way to use v-on

    <button v-on:click="authState" v-else>Login</button>     v-on is how you run js in response to your dom events

    <button @click="counts">count is {{ count }}</button> -->
    <Card title="Hih" desciption="fnj"/>
    
  </div>
</template>

<script>
import Card from "../components/Card.vue";
export default {
  components: {
    Card,
  },
  data(){
    return {
      animals: ["pig", "horse", "donkey", "capybara", "raccoon", "duck"],
      loggedIn: false,
      message: "hello world",
      count: 0,
    };
    return
      cards:[
        {
          name:Cat,
          description:fluffy,
          price: 33,
    
        },
        {
          name:Dog,
          desciption:cute,
          price:36,
        }
      ]
      
    
  },
  methods: {
    authState: function () {
      if(this.loggedIn===false){
      this.loggedIn = true;
    } else {
      this.loggedIn = false;
    }
  },
counts: function(){
  this.count++
},

  },
};

</script>

<style>
.home{
  width:30%;
  background-color: pink;
  height: 500px;
}
</style>


<!-- project should have 2 word components -->



