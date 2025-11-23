<script setup lang="ts">
import { Button } from '@/components/ui/button'
</script>


<template>
  <div>
    <Button variant="destructive" class="px-6 py-3">
  Delete
</Button>
    <h1>Home Page</h1>
    <RouterLink :to="{name: '/projects/[id]', params: {'id': 1}}">Go to Project 1</RouterLink>
  </div>
</template>


