<template>
    <div class="organize">
      <p>{{ event.category }}</p>
      <p>{{ event.organizer }}</p>
    </div>
  </template>
  
  <script setup lang="ts">
  import { type EventItem } from '@/type'
  import { PropType } from 'vue'
  
  const props = defineProps({
    event: {
      type: Object as PropType<EventItem>,
      require: true
    }
  })
  </script>
  
  <style scoped>
  .organize {
    text-align: right;
  }
  </style>