<template>
  <header class="app-header">
    <h1>Task Manager</h1>
  </header>
</template>

<script>
export default {
  name: 'HeaderComp'
}
</script>

<style scoped>
.app-header {
  display: flex;
  justify-content: center; /* Aligns children (h1) horizontally at the center */
  align-items: center;     /* Keeps children (h1) vertically centered */
  background-color: #f5f5f5;
  padding: 10px 20px;
  width: 100%;             /* Ensures the header takes the full width */
}

h1 {
  margin: 0;
  color: #333;
  font-size: 2em;          /* Adjusts font size */
  text-align: center;      /* Ensures text is centered */
  width: 100%;             /* Ensures h1 takes full width of its parent */
  max-width: 600px;        /* Sets a max-width for better readability on large screens */
}
</style>
