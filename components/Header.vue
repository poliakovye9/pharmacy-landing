
import type { NuxtLink } from '#build/components';
<template>
  <Bounded as="header" class="sticky !py-2 md:!py-4 lg:!py-6 z-10">
    <div class="flex gap-4 items-center justify-between flex-col sm:flex-row">
      <Logo class="logo"/>
      <nav>
        <ul class="flex">
          <NuxtLink class="p-4" to="/feature">Features</NuxtLink>
          <NuxtLink class="p-4" to="/about">About</NuxtLink>
        </ul>
      </nav>
    </div>
  </Bounded>
</template>
<style>
  .logo {
    width: 100px;
  }
</style>