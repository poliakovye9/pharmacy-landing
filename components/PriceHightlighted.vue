<template>
  <div
    class="flex flex-col w-5/6 lg:w-1/3 mx-auto lg:mx-0 rounded-lg bg-white mt-4 sm:-mt-6 shadow-lg z-10"
  >
    <div
      class="flex-1 bg-white rounded-t rounded-b-none overflow-hidden shadow"
    >
      <div class="w-full p-8 text-3xl font-bold text-center">{{ name }}</div>
      <div class="h-1 w-full gradient my-0 py-0 rounded-t"></div>
      <ul class="w-full text-center text-base font-bold">
        <li v-for="(item, index) in list" :key="index" class="border-b py-4">
          {{ item }}
        </li>
      </ul>
    </div>
    <div
      class="flex-none mt-auto bg-white rounded-b rounded-t-none overflow-hidden shadow p-6"
    >
      <div class="w-full pt-6 text-4xl font-bold text-center">
        {{ price }}
        <span class="text-base">{{ pricePer }}</span>
      </div>
      <div class="flex items-center justify-center">
        <button
          class="mx-auto lg:mx-0 hover:underline gradient text-white font-bold rounded-full my-6 py-4 px-8 shadow-lg"
        >
          Sign Up
        </button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    name: {
      type: String,
      required: true
    },
    price: {
      type: String,
      required: true
    },
    limited: {
      type: Boolean,
      required: true
    },
    list: {
      type: Array,
      required: true
    }
  }
}
</script>
