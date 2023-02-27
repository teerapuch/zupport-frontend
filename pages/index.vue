<template>
  <div class="flex flex-row">
    <div class="basis-2/4">
      <h1>Let us help you <br />
      <span>Find, Drink, Food</span> <br /> &amp; Meeting</h1>
      <p class="text-xl pr-8">
        บางซื่อ ร้านอาหารเด็ด มากมาย ใครผ่านไปผ่านมาก็อยากให้แวะไปลอง <br /> วันนี้เรารวมมาให้แล้ว กับร้านดังในเขตนี้ ใครสนใจลองส่องเลย
      </p>
      <button class="bg-transparent hover:bg-green-500 text-green-700 font-semibold hover:text-white py-2 px-4 border border-green-500 hover:border-transparent rounded">
        Browse Lists
      </button>
      <button class="ml-5 bg-green-500 hover:bg-bgreenlue-700 text-white font-bold py-2 px-4 border border-green-700 rounded">
        Add Lists
      </button>
    </div>
    <div class="basis-2/4">
      <img src="/assets/banner01.jpg" alt="image" />
    </div>
  </div>
  
  <br />
  <Maps />
  <Getintouch />
  <br />
  <div>
    <div>
      <h1>API Restaurants</h1>
      <!-- 
      <p v-if="$fetchState.pending">Fetching posts...</p>
      <p v-else-if="$fetchState.error">Error while fetching posts: {{ $fetchState.error.message }}</p>
      <ul v-else> 
        <ul>
          <li v-for="restaurant of restaurants">{{ restaurant.title }}</li>
        </ul>
        <button @click="$fetch">Refresh</button>
      -->
    </div>
  </div>
</template>

<script>
export default {
    data() {
      return {
        restaurants: []
      }
    },
    async fetch() {
      this.restaurants = await fetch(
        'http://127.0.0.1:8000/api/restaurant'
      ).then(res => res.json())
    }
  }
</script>

<style scoped>
  h1 {
    font-weight: 800;
    font-size: 50px;
    color: #0D233E;
    margin-bottom: 25px;
  }
  h2 {
    margin-bottom: 20px;
    font-size: 36px;
  }
  p {
    margin: 20px 0;
  }
</style>