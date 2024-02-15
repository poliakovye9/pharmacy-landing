<template>
  <nav :class="headerClassList" class="fixed w-full z-30 top-0">
		<div class="w-full container mx-auto flex flex-wrap items-center justify-between mt-0 py-2">
			<div class="pl-4 flex items-center">
				<Logo :isStickable="true" :isSticky="isSticky" class="logo"/>
			</div>
			<div class="block lg:hidden pr-4">
				<button class="flex items-center p-1 text-orange-800 hover:text-gray-900" @click.prevent.stop="onToggleClick">
					<svg class="fill-current h-6 w-6" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg">
						<title>Menu</title>
						<path d="M0 3h20v2H0V3zm0 6h20v2H0V9zm0 6h20v2H0v-2z" />
					</svg>
				</button>
			</div>
			<div :class="navContentClassList" class="w-full flex-grow lg:items-center lg:w-auto lg:block mt-2 lg:mt-0 bg-white lg:bg-transparent text-black p-4 lg:p-0 z-20">
				<ul class="list-reset lg:flex justify-end flex-1 items-center">
					<li class="mr-3">
						<a class="inline-block py-2 px-4 text-white text-block font-bold no-underline" href="#features">
							Features
						</a>
					</li>
					<li class="mr-3">
						<a class="inline-block text-white no-underline hover:text-gray-800 hover:text-underline py-2 px-4" href="#about">
							About
						</a>
					</li>
				</ul>
			</div>
		</div>
		<hr class="border-b border-gray-400 opacity-25 my-0 py-0" />
	</nav>
</template>



<script lang="ts" setup>

	const scrollY = ref(0)
	const isOpen = ref(false)
  const isSticky = computed(() => scrollY.value > 10)
	const headerClassList = computed(() => isSticky.value ? 'bg-transparent shadow' : '')
	const navActionClassList = computed(() => isSticky.value ? 'gradient text-white' : 'bg-white text-gray-800')
	const navContentClassList = computed(() => {
		let classList = isSticky.value ? 'bg-transparent' : 'bg-gray-100'
		if (!isOpen.value) {
			classList += ` hidden`
		}
		return classList
	})
	const onToggleClick = () => {
		isOpen.value = !isOpen.value
	}
	const onClick = () => {
		isOpen.value = false
	}
	const onScroll = () => {
		scrollY.value = window.scrollY
	}

	onMounted(() => {
		scrollY.value = window.scrollY
		document.addEventListener('click', onClick)
		document.addEventListener('scroll', onScroll)
	})
	onBeforeUnmount(() => {
		document.removeEventListener('click', onClick, true)
		document.removeEventListener('scroll', onScroll, true)
	})
</script>

<style>
.logo {
	width: 96px;
}
</style>

