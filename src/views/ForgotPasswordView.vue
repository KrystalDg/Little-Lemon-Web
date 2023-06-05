<template>
  <div>
    <div
      class="container mt-3 mx-auto px-8 max-w-lg items-center rounded-lg border shadow-xl"
    >
      <h1 class="text-center text-4xl mb-10 pt-10">Forgot password?</h1>
      <form class="relative flex flex-col justify-start space-y-3">
        <div class="field flex flex-col h-16">
          <input
            id="email"
            type="email"
            placeholder=" "
            class="mt-1 rounded-lg border border-gray-200 px-4 pb-2 pt-6 focus:border-zinc-700 outline-none"
          />
          <label
            disabled
            for="email"
            class="absolute mt-1 px-4 pt-4 flex items-center text-lg text-gray-500"
            >Email</label
          >
        </div>
        <div class="button flex justify-center py-4">
          <button
            type="submit"
            class="bg-zinc-700 hover:bg-zinc-800 text-white font-bold py-2 mt-4 px-4 rounded"
          >
            Reset
          </button>
        </div>
        <div class="direction text-center text-zinc-500 pb-10">
          <span class="font-bold m-2">
            <router-link to="/signup">Back</router-link>
          </span>
        </div>
      </form>
    </div>
  </div>
</template>

<script setup>
import { ref } from "vue";
</script>

<style lang="scss" scoped>
.container {
  label {
    transition: all 0.2s ease;
    pointer-events: none;
  }
  input {
    display: block;
    transition: all 0.2s ease;
    &:focus {
      + label {
        transform: translateY(-16px);
        font-size: 12px;
      }
    }
    &:not(:placeholder-shown) {
      + label {
        transform: translateY(-16px);
        font-size: 12px;
      }
    }
  }
}
</style>
