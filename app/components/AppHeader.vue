<script setup lang="ts">
import { NuxtLink } from "#components";

const route = useRoute();
</script>

<template>
  <nav class="background w-full h-[103px]">
    <div
      class="container mx-auto px-[160px] h-full flex justify-between items-center"
    >
      <NuxtLink
        to="/"
        class="text-2xl font-medium flex justify-center items-center gap-4 hover:cursor-pointer"
      >
        <img src="/Group.png" alt="" class="w-[50px] h-[50px]" />FutureTech
      </NuxtLink>
      <ul class="flex justify-between items-center gap-[40px]">
        <NuxtLink
          to="/"
          :class="
            route.path === '/'
              ? 'px-6 py-3 button_back border button_border rounded-[10px]'
              : 'text-neutral-500'
          "
          class="hover:cursor-pointer"
        >
          Home
        </NuxtLink>
        <NuxtLink
          to="/news"
          :class="
            route.path === '/news'
              ? ' px-6 py-3button_back border button_border rounded-[10px]'
              : 'text-neutral-500'
          "
          class="hover:cursor-pointer"
        >
          News
        </NuxtLink>
        <NuxtLink
          to="/podcasts"
          :class="
            route.path === '/podcasts'
              ? 'px-6 py-3 button_back border button_border rounded-[10px]'
              : 'text-neutral-500'
          "
          class="hover:cursor-pointer"
        >
          Podcasts
        </NuxtLink>
        <NuxtLink
          to="/resources"
          :class="
            route.path === '/resources'
              ? 'px-6 py-3 button_back border button_border rounded-[10px]'
              : 'text-neutral-500'
          "
          class="hover:cursor-pointer"
        >
          Resources
        </NuxtLink>
      </ul>
      <div class="flex justify-between items-center gap-10">
        <NuxtLink to="/log-in">Log In</NuxtLink>
        <NuxtLink
          to="/contacts"
          class="py-3 px-5 bg-amber-300 text-black rounded-[10px]"
        >
          Contact Us
        </NuxtLink>
      </div>
    </div>
  </nav>
</template>

<style>
.background {
  background-color: #1a1a1a;
}

.button_back {
  background-color: #141414;
}

.button_border {
  border-color: #333333;
}
</style>
