<template>
  <div>This is a dynamic route : {{ $route.params.id }}</div>

  <div>
    <p>{{ product.title }}</p>
    <p>{{ product.price }}</p>
    <p>{{ product.id }}</p>
  </div>
</template>

<script setup>
  const { id } = useRoute().params
  const uri = 'https://fakestoreapi.com/products/' + id
  //  fetch the products
  const { data: product } = await useFetch(uri, { key: id })
</script>
