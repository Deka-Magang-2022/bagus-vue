<template>
	<main class="w-full min-h-screen bg-blue-100 grid place-items-center">
		<router-view />
		<router-link :to="{ name: 'home' }">
			<div class="font-bold lg:text-xl md:text-lg text-md pr-1">Go Back</div>
		</router-link>	
	</main>
</template>
