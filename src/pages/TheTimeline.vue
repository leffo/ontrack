<script setup>
import TimelineItem from '@/components/TimelineItem.vue'
import { generateTimeLineItems } from '@/functions.js'

const timelineItems = generateTimeLineItems()
</script>

<template>
  <div class="mt-7">
    <ul>
      <TimelineItem  v-for="timelineItem in timelineItems"
                     :key="timelineItem.hour"
                     :timeline-item="timelineItem"
      />
    </ul>
  </div>
</template>

<style scoped>

</style>
