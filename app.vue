<script setup lang="ts">
useHead({
  title: "Sob Ready",
  meta: [
    {
      name: "description",
      content:
        "There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form, by injected humour",
    },
  ],
  bodyAttrs: {
    class: "test",
  },
});

useServerSeoMeta({
  title: "Sob Ready !!!",
  ogTitle: "Fresh Product Directly To Your Door With Free Delivery",
  description:
    "There are many variations of passage Lorem Ipsum available, but te majority hav suffered alteration in some form, by injected humour",
  ogDescription: "Make your online shop sob ready with our mobile all",
  ogImage: "https://example.com/image.png",
  twitterCard: "summary_large_image",
});
</script>

<template>
  <div class="container mx-auto">
    <NuxtLayout>
      <AppNavbar />
      <NuxtPage />
    </NuxtLayout>
  </div>
</template>

<style>
.router-link-active .router-link-exact-active {
  color: #e21a43 !important;
}
</style>
