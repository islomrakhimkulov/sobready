<script setup lang="ts">
const navbarLinks = ref([
  { name: "home", to: "/" },
  { name: "about", to: "/about" },
]);
</script>

<template>
  <div>
    <nav>
      <RouterLink to="/">Sob Ready</RouterLink>
      <ul>
        <li v-for="link in navbarLinks" key="link.name">
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
  </div>
</template>
