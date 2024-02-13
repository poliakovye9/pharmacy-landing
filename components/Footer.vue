
import type { NuxtLink } from '#build/components';
<template>
  <Bounded as="footer" class="!py-4 md:!py-6 lg:!py-8 mt-440">
    <div class="w-full flex justify-center items-center">
      <div class="w-2/3 text-left px-24 py-24 bg-white">
        <div class="title text-center">
          <h1 class="text-4xl text-sky-400">Contact Us</h1>
        </div>
        <div class="q0 block flex flex-col mt-4">
          <label for="q0">Q1. What's your email?</label>
          <input class="bg-gray-300 px-4 py-2 mt-2" type="text" placeholder="Type your email..." />
        </div>
        <div class="q1 block flex flex-col mt-4">
          <label for="q1">Q2. What's your position?</label>
          <input class="bg-gray-300 px-4 py-2 mt-2" type="text" placeholder="Type your position..." />
        </div>
        <div class="q2 block flex flex-col mt-4">
          <label for="q2">Q3. What do you want more in your pharmacy software?</label>
          <text class="bg-gray-300 px-4 py-2 mt-2 min-h-48" type="text" placeholder="List features you need..." />
        </div>
        <div class="submit mt-4 w-full text-center">
          <button type="button" class="bg-sky-400 text-white rounded px-12 py-4">Submit</button>
        </div>
      </div>
    </div>
  </Bounded>
</template>
<style>
  .mt-440 {
    margin-top:440px;
  }
</style>