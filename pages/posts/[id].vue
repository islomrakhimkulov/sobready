<script setup lang="ts">
const { id } = useRoute().params;
</script>

<template>
  <div>Post id: {{ id }}</div>
</template>
