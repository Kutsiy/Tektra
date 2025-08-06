<script setup lang="ts">
const route = useRoute();
</script>

<template>
  <nav class="background w-full h-18">
    <div
      class="container mx-auto px-28 h-full flex justify-between items-center"
    >
      <div class="text-2xl font-medium">FutureTech</div>
      <ul class="flex justify-between items-center gap-10">
        <li
          :class="
            route.path === '/'
              ? 'px-6 py-3 button_back border button_border rounded-[10px]'
              : ''
          "
        >
          Home
        </li>
        <li
          ::class="route.path === '/news' ? 'px-6 py-3 button_back border button_border rounded-[10px]' : ''"
        >
          News
        </li>
        <li
          :class="
            route.path === '/podcasts'
              ? 'px-6 py-3 button_back border button_border rounded-[10px]'
              : ''
          "
        >
          Podcasts
        </li>
        <li
          :class="
            route.path === '/resources'
              ? 'px-6 py-3 button_back border button_border rounded-[10px]'
              : ''
          "
        >
          Resources
        </li>
      </ul>
      <div class="flex justify-between items-center gap-10">
        <div>Log In</div>
        <div class="py-3 px-5 bg-amber-300 text-black rounded-[10px]">
          Contact Us
        </div>
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
