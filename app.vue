<script setup>
definePageMeta({
  title: "My home page",
});
</script>

<template>
  <div>
    <NuxtLayout>
      <div>Some default layout shared across all pages</div>
      <NuxtPage />
      <nav>
        <ul>
          <li><NuxtLink to="/about">About</NuxtLink></li>
          <li><NuxtLink to="/posts/1">Post 1</NuxtLink></li>
          <li><NuxtLink to="/posts/2">Post 2</NuxtLink></li>
        </ul>
      </nav>
    </NuxtLayout>
  </div>
</template>
