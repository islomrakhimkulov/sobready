<script setup lang="ts">
export interface AppInputProps {
  type: string;
  placeholder: string;
}

const props = withDefaults(defineProps<AppInputProps>(), {});
</script>

<template>
  <div>
    <input type="text" class="bg-[##FDE9ED] py-1 px-2" v-model="props" />
  </div>
</template>
