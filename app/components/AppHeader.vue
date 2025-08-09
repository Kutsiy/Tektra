<script setup lang="ts">
import { NuxtLink } from "#components";

const route = useRoute();
</script>

<template>
  <header class="background w-full h-[103px]">
    <nav class="w-full h-full">
      <div
        class="container mx-auto px-[var(--Indent)] h-full flex justify-between items-center"
      >
        <NuxtLink
          to="/"
          class="text-2xl font-medium flex justify-center items-center gap-4 hover:cursor-pointer"
        >
          <img src="/Group.png" alt="" class="w-[50px] h-[50px]" />FutureTech
        </NuxtLink>
        <ul class="flex justify-between items-center gap-[40px] w-[400px]">
          <NuxtLink
            to="/"
            :class="
              route.path === '/'
                ? 'px-6 py-3 link_back border link_border rounded-[10px]'
                : 'not-active'
            "
            class="hover:cursor-pointer"
          >
            Articles
          </NuxtLink>
          <NuxtLink
            to="/news"
            :class="
              route.path === '/Posts'
                ? ' px-6 py-3link_back border link_border rounded-[10px]'
                : 'not-active'
            "
            class="hover:cursor-pointer"
          >
            Posts
          </NuxtLink>
          <NuxtLink
            to="/news"
            :class="
              route.path === '/news'
                ? ' px-6 py-3link_back border link_border rounded-[10px]'
                : 'not-active'
            "
            class="hover:cursor-pointer"
          >
            News
          </NuxtLink>
          <NuxtLink
            to="/podcasts"
            :class="
              route.path === '/podcasts'
                ? 'px-6 py-3 link_back border link_border rounded-[10px]'
                : 'not-active'
            "
            class="hover:cursor-pointer"
          >
            Podcasts
          </NuxtLink>
        </ul>
        <div class="flex justify-between items-center gap-10">
          <NuxtLink to="/log-in">Log In</NuxtLink>
          <NuxtLink to="/sign-up" class="py-3 px-5 rounded-[10px] button">
            Sign Up
          </NuxtLink>
        </div>
      </div>
    </nav>
  </header>
</template>

<style scoped>
.background {
  background-color: var(--Dark-10);
}

.not-active {
  color: var(--Gray-50);
}

.button {
  background-color: var(--Yellow-55);
  color: var(--Dark-08);
}

.link_back {
  background-color: var(--Dark-08);
}

.link_border {
  border-color: var(--Dark-20);
}
</style>
