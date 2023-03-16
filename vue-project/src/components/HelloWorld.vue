<template>
  <div class="home">
    <h1 v-if="graduated">{{ student }}</h1>
    <h1 v-else="graduated">They did not yet graduate</h1>  
    <h1 :class="titleClass">{{ message }}</h1>
    <h2 v-if="latePractice">{{ message2 }}</h2>
    <h2 v-else>cons- not going to practice at all with the lines that we put down, not use to own courts, far away, hungry</h2>
    <ul>
      <li v-for="animal in animals" :key="animal">{{ animal }}</li>
    </ul>
    <button @click="authState" v-if="loggedIn">Log Out</button>    <!-- @ = src, quicker way to use v-on -->

    <button v-on:click="authState" v-else>Login</button>     <!-- v-on is how you run js in response to your dom events -->

    <button @click="counts">count is {{ count }}</button>
  </div>
</template>

<script>

export default {
  name: "Home", 
  components: {},
  data(){
    return {
      student: "Harry",
      graduated: true,
      animals: ["pig", "horse", "donkey", "capybara", "raccoon", "duck"],
      loggedIn: false,
      message: "hello world",
      titleClass: "title",
      count: 0,
      latePractice: true,
      message2: "pros- you can get food, you can study, don't need to travel to ps50, use the hardworking lines we put down, get use to our own school's courts",
    };
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

<style scoped>
.title{
  color:red;
}
</style>
<!-- project should have 2 word components -->



