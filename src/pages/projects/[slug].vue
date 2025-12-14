<script setup lang="ts">
const route = useRoute()
</script>

<template>
  <div>
    <h2>Project Name {{ route.params?.slug }}</h2>
  </div>
</template>
