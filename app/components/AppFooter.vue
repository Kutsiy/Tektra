import { Icon, componentNames } from '../../.nuxt/components';
<script></script>

<template>
  <footer class="w-full bg-[var(--Dark-10)]">
    <nav class="w-full h-full px-[var(--Indent)] py-[80px] flex gap-[80px]">
      <div class="w-[255px]">
        <h4>Home</h4>
        <ul class="flex flex-col mt-[36px] gap-[18px] text-[var(--Dark-40)]">
          <NuxtLink>Articles</NuxtLink>
          <NuxtLink>Posts</NuxtLink>
          <NuxtLink>News</NuxtLink>
          <NuxtLink>Podcasts</NuxtLink>
          <NuxtLink>Log In</NuxtLink>
          <NuxtLink>Sign Up</NuxtLink>
        </ul>
      </div>
      <div class="w-[255px]">
        <h4>Posts</h4>
        <ul class="flex flex-col mt-[36px] gap-[18px] text-[var(--Dark-40)]">
          <NuxtLink></NuxtLink>
          <NuxtLink></NuxtLink>
          <NuxtLink></NuxtLink>
          <NuxtLink></NuxtLink>
          <NuxtLink></NuxtLink>
        </ul>
      </div>
      <div class="w-[255px]">
        <h4>News</h4>
        <ul class="flex flex-col mt-[36px] gap-[18px] text-[var(--Dark-40)]">
          <NuxtLink></NuxtLink>
          <NuxtLink></NuxtLink>
          <NuxtLink></NuxtLink>
          <NuxtLink></NuxtLink>
          <NuxtLink></NuxtLink>
        </ul>
      </div>
      <div class="w-[255px]">
        <h4>Podcasts</h4>
        <ul class="flex flex-col mt-[36px] gap-[18px] text-[var(--Dark-40)]">
          <NuxtLink></NuxtLink>
          <NuxtLink></NuxtLink>
          <NuxtLink></NuxtLink>
          <NuxtLink></NuxtLink>
          <NuxtLink></NuxtLink>
        </ul>
      </div>
      <div class="w-[255px]">
        <h4>Contacts</h4>
        <ul class="flex flex-col mt-[36px] gap-[18px] text-[var(--Dark-40)]">
          <NuxtLink></NuxtLink>
          <NuxtLink></NuxtLink>
          <NuxtLink></NuxtLink>
          <NuxtLink></NuxtLink>
          <NuxtLink></NuxtLink>
        </ul>
      </div>
    </nav>
    <div class="w-full h-[103px] px-[var(--Indent)]">
      <div class="top-border flex justify-between items-center w-full h-full">
        <div class="flex gap-[11px]">
          <div class="text-[var(--Dark-40)]">Terms & Conditions</div>
          <div
            style="border-left: 3px solid var(--Dark-15)"
            class="pl-[11px] text-[var(--Dark-40)]"
          >
            Privacy Policy
          </div>
        </div>
        <div class="flex gap-[20px]">
          <Icon name="mdi:twitter" style="font-size: 22px" />
          <Icon name="mage:medium" style="font-size: 22px" />
          <Icon name="mdi:linkedin" style="font-size: 22px" />
        </div>
        <div class="text-[var(--Dark-40)]">
          @ 2025 FutureTech. All rights reserved.
        </div>
      </div>
    </div>
  </footer>
</template>

<style scoped>
.top-border {
  border-top: 3px solid var(--Dark-15);
}
</style>
