<template>
  <div>This is index posts</div>
    <div v-for="p in products">
      <NuxtLink :to="`/posts/${p.id}`">{{ p.title }}</NuxtLink>
    </div>
</template>

<script setup>
  //  fetch the products
  const { data: products } = await useFetch('https://fakestoreapi.com/products')
</script>