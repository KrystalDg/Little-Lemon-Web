<template>
  <div class="container flex flex-col items-center">
    <div class="feature-img mb-6">
      <img class="max-h-72" :src="item.img" alt="" />
    </div>
    <div class="feature-title text-center">
      <h3 class="text-xl">{{ item.title.toUpperCase() }}</h3>
      <router-link to="/">
        <button class="border border-zinc-500 px-1 py-1 text-xs rounded mt-6">
          {{ item.button.toUpperCase() }}
        </button>
      </router-link>
    </div>
  </div>
</template>

<script setup>
defineProps({
  item: Object,
});
</script>

<style lang="scss" scoped></style>
