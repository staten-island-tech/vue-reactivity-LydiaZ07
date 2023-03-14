<template>
  <div class="home">
    <h1 v-if="graduated">{{ student }}</h1>
    <h1 v-else="graduated">They did not yet graduate</h1>  
    <ul>
      <li v-for="animal in animals" :key="animal">{{ animal }}</li>
    </ul>
  </div>
</template>

<script>

export default {
  name: "Home", 
  components: {},
  data(){
    return {
      student: "Harry",
      graduated: false,
      animals: ["pig", "horse", "donkey", "capybara", "raccoon", "duck"],
    };
  },
};

</script>




