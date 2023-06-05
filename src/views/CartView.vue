<template>
  <div>
    <div class="cart-empty px-28 py-32 mb-16">
      <div class="title text-center text-6xl mb-10 pt-10">
        <h1>Your Cart</h1>
      </div>
      <div class="body-cart text-center text-xl flex flex-col justify-center">
        <p>Your cart is empty</p>

        <router-link
          to="/products"
          class="back-button flex justify-center py-4 text-sm"
        >
          <button
            class="flex bg-zinc-700 hover:bg-zinc-800 text-white font-bold py-2 px-4 rounded"
          >
            <span class="flex items-center"> GO SHOPPING </span>
            <span class="flex items-center">
              <svg class="search fill-current ml-1 h-5 w-5" viewBox="0 0 20 8">
                <path
                  fill-rule="evenodd"
                  clip-rule="evenodd"
                  d="M15.186.445c.865.944 1.614 1.662 2.246 2.154.631.491 1.227.857 1.787 1.098v.44a9.933 9.933 0 0 0-1.875 1.196c-.606.485-1.328 1.196-2.168 2.134h-.752c.612-1.309 1.253-2.315 1.924-3.018H.77v-.986h15.577c-.495-.632-.84-1.1-1.035-1.406-.196-.306-.486-.843-.87-1.612h.743z"
                ></path>
              </svg>
            </span>
          </button>
        </router-link>
      </div>
    </div>
    <div class="cart-items"></div>
  </div>
</template>

<script setup>
import { RouterLink } from "vue-router";
</script>
