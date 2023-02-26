<template>
  <div>
    <header class="shadow-sm bg-white">
      <nav class="container mx-auto p-4 flex justify-between">
        <NuxtLink to="/" class="font-bold">Restaurant</NuxtLink>
        <ul class="flex gap-4">
          <li><NuxtLink to="/about" class="bg-transparent hover:bg-green-500 text-green-700 font-semibold hover:text-white py-2 px-4 border border-green-500 hover:border-transparent rounded">About</NuxtLink></li>
          <li><NuxtLink to="/restaurants/" class="bg-transparent hover:bg-green-500 text-green-700 font-semibold hover:text-white py-2 px-4 border border-green-500 hover:border-transparent rounded">Restaurant</NuxtLink></li>
          <li><NuxtLink to="/posts/">Posts</NuxtLink></li>
          <li><NuxtLink to="/posts/1">Post 1</NuxtLink></li>
          <li><NuxtLink to="/posts/2">Post 2</NuxtLink></li>
        </ul>
      </nav>
    </header>
    <div class="container mx-auto p-4">
      <slot />
    </div>
    <footer class="text-center">Footer goes here</footer>
  </div>
</template>

<style scoped>
.router-link-exact-active {
    color: #12b488;
  }
</style>