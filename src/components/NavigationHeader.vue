<template>
  <header>
    <div class="grid grid-cols-7 mx-12 items-center">
      <div class="nav-logo w-24 col-span-3">
        <router-link to="/">
          <img class="max-w-full" src="../assets/icons/logo.avif" alt="logo" />
        </router-link>
      </div>
      <nav class="nav-menu text-lg col-span-3">
        <router-link class="px-3 py-1" to="/">Home</router-link>
        <router-link class="px-3 py-1" to="/products">Products</router-link>
      </nav>
      <div class="nav-button grid grid-cols-3 items-center justify-end">
        <button class="search-button">
          <svg
            class="search ml-3 h-5 w-5 fill-current"
            viewBox="0 0 18 19"
            fill="none"
          >
            <path
              fill-rule="evenodd"
              clip-rule="evenodd"
              d="M11.03 11.68A5.784 5.784 0 112.85 3.5a5.784 5.784 0 018.18 8.18zm.26 1.12a6.78 6.78 0 11.72-.7l5.4 5.4a.5.5 0 11-.71.7l-5.41-5.4z"
            ></path>
          </svg>
        </button>
        <router-link to="/login">
          <svg
            class="login-button ml-3 h-5 w-5 fill-current"
            viewBox="0 0 18 19"
            fill="none"
          >
            <path
              fill-rule="evenodd"
              clip-rule="evenodd"
              d="M6 4.5a3 3 0 116 0 3 3 0 01-6 0zm3-4a4 4 0 100 8 4 4 0 000-8zm5.58 12.15c1.12.82 1.83 2.24 1.91 4.85H1.51c.08-2.6.79-4.03 1.9-4.85C4.66 11.75 6.5 11.5 9 11.5s4.35.26 5.58 1.15zM9 10.5c-2.5 0-4.65.24-6.17 1.35C1.27 12.98.5 14.93.5 18v.5h17V18c0-3.07-.77-5.02-2.33-6.15-1.52-1.1-3.67-1.35-6.17-1.35z"
            ></path>
          </svg>
        </router-link>
        <router-link to="/cart">
          <svg
            class="cart-button h-10 w-10 fill-current"
            viewBox="0 0 40 40"
            fill="none"
          >
            <path
              fill-rule="evenodd"
              d="m15.75 11.8h-3.16l-.77 11.6a5 5 0 0 0 4.99 5.34h7.38a5 5 0 0 0 4.99-5.33l-.78-11.61zm0 1h-2.22l-.71 10.67a4 4 0 0 0 3.99 4.27h7.38a4 4 0 0 0 4-4.27l-.72-10.67h-2.22v.63a4.75 4.75 0 1 1 -9.5 0zm8.5 0h-7.5v.63a3.75 3.75 0 1 0 7.5 0z"
            ></path>
          </svg>
        </router-link>
      </div>
    </div>
  </header>
</template>

<script setup>
import { RouterLink } from "vue-router";
</script>
