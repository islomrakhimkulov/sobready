<script setup lang="ts">
const props = defineProps({
  id: {
    type: Number,
  },
});
</script>

<template>
  <div>Post id: {{ props.id }}</div>
</template>
