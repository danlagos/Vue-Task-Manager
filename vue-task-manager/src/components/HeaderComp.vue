<template>
  <header class="app-header">
    <h1>Task Manager</h1>
    <nav class="navigation-bar">
      <RouterLink to="/" class="nav-link">All</RouterLink> |
      <RouterLink to="/active" class="nav-link">Active</RouterLink> |
      <RouterLink to="/completed" class="nav-link">Completed</RouterLink> |
      <RouterLink to="/important" class="nav-link">Important</RouterLink>
    </nav>
  </header>
</template>

<script>
import { RouterLink } from 'vue-router' // Import RouterLink for navigation

export default {
  name: 'HeaderComp'
}
</script>

<style scoped>
.app-header {
  display: flex;
  flex-direction: column;
  align-items: center;
  background-color: #000; /* Bold black background */
  padding: 20px 40px; /* Adds padding on both sides */
  width: 100%; /* Ensures the header takes the full width */
}

h1, .navigation-bar {
  width: 100%; /* Ensures content uses the full available width */
  text-align: center;
}

h1 {
  margin: 0;
  color: #FFF; /* High-contrast white text */
  font-size: 2em;
}

.navigation-bar {
  margin-top: 10px;
}

.nav-link {
  color: #FFF; /* White text for high readability */
  text-decoration: none; /* No underline for a cleaner look */
  padding: 5px 10px; /* Padding for better link tap area */
  transition: color 0.3s; /* Smooth transition for hover effects */
}

.nav-link:hover {
  color: #9B59B6; /* Lighter purple on hover for emphasis */
}
</style>

