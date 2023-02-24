<template>
  <div>This is index</div>
  <!-- Components -->
  <AppAlert>
    This is an auto-imported App Alert component.
  </AppAlert>
  <br />
  <img src="/assets/unsplash01.jpg" alt="image" />
  <br />
  <Counter />
  <br />
  <h1>{{ organization.login }}</h1>
  <p>{{ organization.description }}</p>
</template>

<script>

export default defineComponent({
  async setup() {
    const [{ data: organization }, { data: repos }] = await Promise.all([
      useFetch(`https://api.github.com/orgs/nuxt`),
      useFetch(`https://api.github.com/orgs/nuxt/repos`)
    ])
    return {
      organization,
      repos
    }
  }
})


</script>
