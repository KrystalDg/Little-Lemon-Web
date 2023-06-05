<template>
  <div class="app-wrapper">
    <div class="app">
      <navigation-header />
      <router-view />
      <navigation-footer />
    </div>
  </div>
</template>

<script setup>
import { RouterLink, RouterView } from "vue-router";

import NavigationHeader from "./components/NavigationHeader.vue";
import NavigationFooter from "../src/components/NavigationFooter.vue";
</script>

<style scoped></style>
