<template>
  <div>
    <div
      class="container mt-3 mx-auto px-8 max-w-lg items-center rounded-lg border shadow-xl"
    >
      <h1 class="text-center text-4xl mb-10 pt-10">Create Account</h1>
      <form class="flex flex-col justify-start space-y-3">
        <div class="full-name grid grid-cols-2 gap-10">
          <div class="field flex flex-col">
            <input
              id="firstname"
              type="text"
              placeholder=" "
              class="mt-1 rounded-lg border border-gray-200 px-4 pb-2 pt-6 focus:border-zinc-700 outline-none"
            />
            <label
              for="firstname"
              class="absolute mt-1 px-4 pt-4 flex items-center text-lg text-gray-500"
              >First Name</label
            >
          </div>
          <div class="field flex flex-col">
            <input
              id="lastname"
              type="text"
              placeholder=" "
              class="mt-1 rounded-lg border border-gray-200 px-4 pb-2 pt-6 focus:border-zinc-700 outline-none"
            />
            <label
              for="lastname"
              class="absolute mt-1 px-4 pt-4 flex items-center text-lg text-gray-500"
              >Last Name</label
            >
          </div>
        </div>
        <div class="field flex flex-col">
          <input
            id="username"
            type="text"
            placeholder=" "
            class="mt-1 rounded-lg border border-gray-200 px-4 pb-2 pt-6 focus:border-zinc-700 outline-none"
          />
          <label
            for="username"
            class="absolute mt-1 px-4 pt-4 flex items-center text-lg text-gray-500"
            >Username</label
          >
        </div>
        <div class="field flex flex-col">
          <input
            id="email"
            type="email"
            placeholder=" "
            class="mt-1 rounded-lg border border-gray-200 px-4 pb-2 pt-6 focus:border-zinc-700 outline-none"
          />
          <label
            for="email"
            class="absolute mt-1 px-4 pt-4 flex items-center text-lg text-gray-500"
            >Email</label
          >
        </div>
        <div class="field flex flex-col">
          <input
            id="password"
            type="password"
            placeholder=" "
            class="mt-1 rounded-lg border border-gray-200 px-4 pb-2 pt-6 focus:border-zinc-700 outline-none"
          />
          <label
            for="password"
            class="absolute mt-1 px-4 pt-4 flex items-center text-lg text-gray-500"
            >Password</label
          >
        </div>
        <div class="field flex flex-col">
          <input
            id="confirmpassword"
            type="password"
            placeholder=" "
            class="mt-1 rounded-lg border border-gray-200 px-4 pb-2 pt-6 drop-shadow focus:border-zinc-700 outline-none"
          />
          <label
            for="confirmpassword"
            class="absolute mt-1 px-4 pt-4 flex items-center text-lg text-gray-500"
            >Confirm Password</label
          >
        </div>
        <div class="button flex justify-center py-4">
          <button
            type="submit"
            class="bg-zinc-700 hover:bg-zinc-800 text-white font-bold py-2 px-4 rounded"
          >
            Sign Up
          </button>
        </div>
        <div class="direction text-center pb-10">
          <span>Already on LittleLemon?</span>
          <span class="font-bold m-2">
            <router-link to="/login">Sign In</router-link>
          </span>
        </div>
      </form>
    </div>
  </div>
</template>

<script setup>
import { ref } from "vue";
import { RouterLink } from "vue-router";
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
