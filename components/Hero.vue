
import type { Clinic } from '#build/components';

import type { Disease } from '#build/components';
<template>
  <div id="hero" class="relative text-center min-h-screen inset-0 bg-gradient-to-r from-sky-400 to-white to-top flex justify-center items-center">
    <div class="w-5/6 md:w-11/12 flex justify-center">
      <div class="w-full flex flex-col md:flex-row">
        <div class="p-4 md:w-1/2">
          <img class="hero_doctor" src="~/assets/images/doctor.png" alt="Doctor" />
        </div>
        <div class="relative px-4 py-24 md:py-12 sm:py-4 md:w-1/2 text-left max-w-screen-md ">
          <div class="absolute top-48 md:top-24 sm:top-12">
            <h3 class="text-9xl text-sky-400 md:text-5xl sm:text-lg font-bold">
              We need your valuable suggestions to improve
            </h3>
            <p class="text-4xl pt-12 md:pt-6 font-light md:text-lg sm:text-base">
              We need your feedback and we want to explain our pharmacy software to you. We need to
              know the problems you have been facing with the software you have been using so we can
              resolve them for you. We don’t want you to spend anything at the moment but help us build a
              product that is designed according to your pharmacy needs. Let's schedule a 1:1 interaction to
              cater to your requirements because we want to be a part of this product.
            </p>
            <div class="mt-8 md:mt-6 sm:w-full">
              <button type="button" class="bg-transparent text-4xl md:text-lg hover:bg-sky-400 border-2 border-sky-400 text-sky-400 font-bold py-2 px-8 rounded cursor-pointer">Tell us</button>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="absolute bg-sky-400 w-2/3 bottom-60 px-12 py-8">
      <div class="w-full flex flex-col md:flex-row">
        <div class="flex p-4 md:w-1/2">
          <Disease />
          <div class="text-left pl-12 pr-4">
            <h1 class="text-white text-4xl">MEDICAL CARE</h1>
            <p class="text-white">Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt</p>
          </div>
        </div>
        <div class="flex p-4 md:w-1/2">
          <Clinic />
          <div class="text-left pl-12 pr-4">
            <h1 class="text-white text-4xl">CARE PROGRAMS</h1>
            <p class="text-white">Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<style>
.to-top {
  margin-top: -100px;
  padding-top: 100px;
}
.hero_doctor {
  width: 80%;
}
</style>
