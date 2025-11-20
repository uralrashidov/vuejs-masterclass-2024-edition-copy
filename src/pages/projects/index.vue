<script setup lang="ts">
  import { supabase } from '@/lib/supabaseClient';
  import { ref } from 'vue';

  const projects = ref();

  (async () => {
    const { data, error } = await supabase.from('projects').select();
    if (error) {
      console.error(error);
    } else {
      projects.value = data;
      console.log('Projects : ', projects.value);
    }
  })();
</script>

<template>
  <div>
    <h1>Projects Page</h1>
    {{ projects }}
    <RouterLink to="/">Go to Home</RouterLink>
  </div>
</template>


