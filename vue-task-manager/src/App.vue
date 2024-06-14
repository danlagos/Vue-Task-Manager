<script setup>
import { RouterLink, RouterView } from 'vue-router'

</script>

<template>
  <header>
    <div class="layout">
      <nav>
        <RouterLink to="/">Home</RouterLink> |
        <RouterLink to="/app-view">App View</RouterLink> |
        <RouterLink to="/about">About</RouterLink> |
      </nav>
    </div>
  </header>

  <RouterView />
</template>

<style scoped>
.layout {
  display: flex;
  justify-content: center; /* Center horizontally within the layout div */
  width: 100%; /* Take full width to allow centering */
}

nav {
  text-align: center; /* Centers text links within the nav element */
  padding: 10px; /* Provides some spacing */
}
</style>
