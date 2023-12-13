<script setup>
const { data: scizor } = await useFetch('/api/scizor')
</script>
<template>
  <h1>Home Page for Nuxt 3 Server</h1>
  <ul>
    <li>
      <img :src="scizor.sprite">
    </li>
    <li>{{ scizor.id }}: {{ scizor.name }}</li>
  </ul>
</template>