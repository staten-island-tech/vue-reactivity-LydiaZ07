<template>
  <div class="home">
    <h1 v-if="graduated">{{ student }}</h1>
    <h1 v-else="graduated">They did not yet graduate</h1>  
    <ul>
      <li v-for="animal in animals" :key="animal">{{ animal }}</li>
    </ul>
    <button @click="authState" v-if="loggedIn">Log Out</button>
    <button v-on:click="authState" v-else>Login</button>
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
  }
};

</script>

<!-- project should have 2 word components -->



