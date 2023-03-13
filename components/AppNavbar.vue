<script setup lang="ts">
const navbarLinks = ref([
  { name: "Home", to: "/" },
  { name: "About", to: "/about" },
  { name: "Category", to: "/category" },
  { name: "Shop", to: "/shop" },
  { name: "Blog", to: "/blog" },
  { name: "Page", to: "/page" },
]);
</script>

<template>
  <nav class="flex items-center justify-between py-5">
    <RouterLink to="/" class="font-semibold uppercase">
      <span class="text-[#E21A43]">Sob</span> Ready
    </RouterLink>
    <ul class="flex items-center gap-8">
      <li class="flex flex-row" v-for="link in navbarLinks" key="link.name">
        <RouterLink :to="link.to">{{ link.name }}</RouterLink>
      </li>
    </ul>
    <div>
      <div>
        <input
          type="text"
          class="p-2 bg-pink-300 text-white"
          placeholder="Search..."
        />
        <RouterLink to="" class="btn">Link</RouterLink>
      </div>
    </div>
  </nav>
</template>

<style>
.router-link-active .router-link-exact-active {
  color: #e21a43 !important;
}
</style>
