<script setup lang="ts">
import { useRoute } from 'vue-router';
const route = useRoute();
</script>

<template>
  <div>
    <h2>Project Name {{ route.params?.id }} </h2>
  </div>
</template>
