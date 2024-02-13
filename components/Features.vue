<template>
  <div class="w-full flex flex-col md:flex-row bg-white py-20 max-h-screen min-h-200">
    <div class="flex p-4 w-1/2 md:w-1/2">
      <div class="content px-48">
        <h1 class="text-4xl text-sky-400">Smooth Pharmacy Software</h1>
        <p class="mt-12 text-neutral-700">Smooth Pharmacy is aimed at introducing an industry leading pharmacy software in the USA. A
          cloud based software to remove any kind of CD installations, update issues, or crashes.
          Designed specifically according to the pharmacy role(pharmacist, technician, manager, owner)
          to harness the power of customization. Yes, no more boring screens with hundreds of
          checkboxes but a smooth software experience that can be customized by you or your team.
        </p>
        <div class="mt-8 md:mt-6 sm:w-full">
          <button type="button" class="bg-transparent text-4xl md:text-lg hover:bg-sky-400 border-2 border-sky-400 text-sky-400 font-bold py-2 px-8 rounded cursor-pointer">Go To Next</button>
        </div>
      </div>
    </div>
    <div class="flex p-4 w-1/2 md:w-1/2 relative">
      <img class="right-0 absolute h-full"src="~/assets/images/computer.jpg" alt="Computer" />
    </div>
  </div>
</template>
<style>
.min-h-200 {
  min-height: 50rem;
}
</style>