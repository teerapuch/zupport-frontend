<template>
  <div>
    <header>
      <nav>
        <ul>
          <li><NuxtLink to="/about" class="test">About</NuxtLink></li>
          <li><NuxtLink to="/posts/">Posts</NuxtLink></li>
          <li><NuxtLink to="/posts/1">Post 1</NuxtLink></li>
          <li><NuxtLink to="/posts/2">Post 2</NuxtLink></li>
        </ul>
      </nav>
      <h1>Header goes here</h1>
    </header>
      <slot />
    <footer>Footer goes here</footer>
  </div>
</template>