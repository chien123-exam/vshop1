<template>
<div class="antialiased bg-gray-50 dark:bg-gray-900">
    <Narbar />

    <Sidebar />
    
    <slot />
  </div>
</template>

<script setup>
import { onMounted } from 'vue'
import { initFlowbite } from 'flowbite'
import Narbar from './Narbar.vue'
import Sidebar from './Sidebar.vue'

// initialize components based on data attribute selectors
onMounted(() => {
    initFlowbite();
})
</script>

