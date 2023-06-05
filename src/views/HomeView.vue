<template>
  <div class="container">
    <div class="cover-1 relative text-center text-white mx-auto">
      <div class="cover-background absolute w-full">
        <div class="cover-content absolute w-full top-1/2">
          <h2 class="text-7xl mb-4">Little Lemon</h2>
          <div class="text-2xl mx-auto">
            <p>Custom Blythe dolls & clothes</p>
          </div>
        </div>
      </div>
    </div>
    <div class="content px-40 py-20">
      <div class="feature-items my-20">
        <div class="wraper flex flex-wrap justify-between">
          <div class="feature-item" v-for="item in FEATURE_ITEMS">
            <feature-item :item="item" />
          </div>
        </div>
      </div>
      <div class="collection py-16">
        <div class="tile text-center text-3xl mb-14">
          <h2>BLYTHE DOLLS FOR ADOPTION</h2>
        </div>
        <div class="wraper px-14 flex flex-wrap justify-between mb-12">
          <collection-item />
          <collection-item />
          <collection-item />
        </div>
        <div class="flex justify-center">
          <router-link
            to="/"
            class="rounded border bg-zinc-700 px-3 py-2 text-white"
          >
            VIEW ALL
          </router-link>
        </div>
      </div>
      <div class="collection py-16">
        <div class="tile text-center text-3xl mb-14">
          <h2>OTHER DOLLS FOR ADOPTION</h2>
        </div>
        <div class="wraper px-14 flex flex-wrap justify-between mb-12">
          <collection-item />
          <collection-item />
          <collection-item />
        </div>
        <div class="flex justify-center">
          <router-link
            to="/"
            class="rounded border bg-zinc-700 px-3 py-2 text-white"
          >
            VIEW ALL
          </router-link>
        </div>
      </div>
      <div class="collection py-16">
        <div class="tile text-center text-3xl mb-14">
          <h2>CLOTHES FOR BLYTHE DOLL</h2>
        </div>
        <div class="wraper px-14 flex flex-wrap justify-between mb-12">
          <collection-item />
          <collection-item />
          <collection-item />
        </div>
        <div class="flex justify-center">
          <router-link
            to="/"
            class="rounded border bg-zinc-700 px-3 py-2 text-white"
          >
            VIEW ALL
          </router-link>
        </div>
      </div>
      <div class="blog grid grid-cols-2 gap-20">
        <div class="image flex justify-end">
          <img
            class="max-h-80"
            src="../assets/images/custom-blythe-doll-little-lemon-sarah-shade-1_345x345@2x.webp"
            alt=""
          />
        </div>
        <div class="title">
          <h2>LEMON'S BLOG</h2>
          <div class="flex justify-start">
            <router-link
              to="/"
              class="rounded border bg-zinc-700 px-3 py-2 text-white"
            >
              VIEW ALL
            </router-link>
          </div>
        </div>
      </div>
    </div>
    <div class="cover-2"></div>
  </div>
</template>

<script setup>
import { RouterLink } from "vue-router";
import FeatureItem from "../components/FeatureItem.vue";
import CollectionItem from "../components/CollectionItem.vue";
import { FEATURE_ITEMS } from "../constants";
</script>

<style lang="scss" scoped>
.container {
  .cover-1 {
    background-image: url("../assets/images/hoffman_sin_logo_1_1296x.webp");
    height: 40vw;
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;

    .cover-background {
      height: 40vw;
      background: rgb(0, 0, 0);
      background: rgba(93, 85, 85, 0.4);
      color: #f1f1f1;

      .cover-content {
        padding: 0px;
      }
    }
  }
  .feature-columns {
    .feature-img {
      img {
        max-width: 400px;
        max-height: 345px;
      }
    }
  }
}
</style>
