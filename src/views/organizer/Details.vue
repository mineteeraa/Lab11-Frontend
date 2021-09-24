<template>
  <img v-for="url in organizer.imageUrls" :key="url" :src="url" />
  <p>{{ organizer.name }}</p>
</template>

<script>
export default {
  props: ['organizer']
}
</script>

<style scoped>
img {
  border: 1px solid #ddd; /* Gray border */
  border-radius: 4px; /* Rounded border */
  padding: 5px; /* Some padding */
  margin: 5px; /* Some margin */
  width: 200px; /* Set a small width */
}
/* Add a hover effect (blue shadow) */
img:hover {
  box-shadow: 0 0 2px 1px rgba(0, 140, 186, 0.5);
}
</style>