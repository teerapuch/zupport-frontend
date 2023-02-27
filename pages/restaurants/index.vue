<template>
  <div>This is index Restaurant</div>
  
</template>

<script>

export default defineComponent({
  async setup() {
    const [{ data: restaurant }] = await Promise.all([
      useFetch(`http://127.0.0.1:8000/api/restaurant`)
    ])
    return {
      restaurant
    }
  }
})
</script>