<template>
  <div class="hello">
    {{foodItem}}
    <img :src="tacoImage" alt="tacos">
    {{price}}
    <button @click="buy">BUY</button>
   
  </div>
</template>

<script>
export default {
  name: 'HomeComponent',
  data() {
    return {
      foodItem: 'Taco Lunch',
      tacoImage:'https://cdn-jaxrestaurant.pressidium.com/wp-content/uploads/2015/05/Corner-Taco-Lunch-1024x791.jpg',
      price: 3.99,
    }
  },
  methods: {
    buy(){
      this.price--
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>

</style>
