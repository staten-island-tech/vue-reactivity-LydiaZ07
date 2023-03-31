<template>
  <div class="home">
 
    <h1>hi</h1>
  <div class="cards">
    <Card v-for="(product, index) in products"
    :key="index"
    :title="product.name"
    :cost="product.cost"
    :img="product.img">
    </Card>
  </div>
    
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
      products: [
          {
            quantity: 1,
            name: "Bear",
            cost: 10,
            img: "https://cdn3.volusion.com/9nxdj.fchy5/v/vspfiles/photos/AR-01779-2.jpg?v-cache=1673333887",
          },
          {
            quantity: 1,
            name: "Rabbit",
            cost:  10,
            img: "https://images.heb.com/is/image/HEBGrocery/005642041?fit=constrain,1&wid=800&hei=800&fmt=jpg&qlt=85,0&resMode=sharp2&op_usm=1.75,0.3,2,0",
          },
          {
            quantity: 1,
            name: "Cat",
            cost:  10,
            img: "https://assets.pkimgs.com/pkimgs/ab/images/dp/wcm/202308/0070/cozy-critter-cat-plush-o.jpg",
          },
          {
            quantity: 1,
            name: "Dog",
            cost:  10,
            img: "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQcimBWR4C3m8HxE3amDvudDGdSnZOHGmi4Ew&usqp=CAU",
          },
          {
            quantity: 1,
            name: "Pig",
            cost:  10,
            img: "https://www.cyrenanime.com/storage/product-photos/63/soft-squishy-pig-plush-doll-white-6-inches-kawaii-plushie.jpg",
          },
          {
            quantity: 1,
            name: "Panda",
            cost: 10,
            img: "https://m.media-amazon.com/images/W/IMAGERENDERING_521856-T1/images/I/61x1q3ZUslL.jpg",
          },
          {
            quantity: 1,
            name: "Snake",
            cost:  10,
            img: "https://m.media-amazon.com/images/W/IMAGERENDERING_521856-T1/images/I/61ZRlCm334L.jpg",
          },
          {
            quantity: 1,
            name: "Bird",
            cost:  10,
            img: "https://cdn3.volusion.com/9nxdj.fchy5/v/vspfiles/photos/WR-18230-2.jpg?v-cache=1673333887",
          },
          {
            quantity: 1,
            name: "Whale",
            cost: 10,
            img:"https://m.media-amazon.com/images/W/IMAGERENDERING_521856-T1/images/I/61LFrb06wvL.jpg",
          },
          {
            quantity: 1,
            name: "Cow",
            cost: 10,
            img: "https://m.media-amazon.com/images/I/61oFdymjRKL._AC_SX425_.jpg",
          },
          {
            quantity: 1,
            name: "Sheep",
            cost: 10,
            img:"http://cdn.shopify.com/s/files/1/0139/0811/5514/products/106071-Shep-the-Sheep-2.jpg?v=1645435675",
          },
          {
            quantity: 1,
            name: "Capybara",
            cost: 10,
            img: "https://cdn.shopify.com/s/files/1/0957/5750/products/PLUSHCAPYBARA1410050091662575_1200x.jpg?v=1678470054",
          },
        ],
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

<style>
.home{
  width:30%;
  background-color: pink;
  height: 500px;
}
</style>


<!-- project should have 2 word components -->



