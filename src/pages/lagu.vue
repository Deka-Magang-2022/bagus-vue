<script setup lang="ts">
	useHead({
		title: 'Lagu',
	});
</script>

<template>
	<div class="flex flex-col gap-5">
		<p>Cari Sendiri</p>
		<audio controls>
		  	<source src="/src/assets/konig.ogg" type="audio/ogg">
			<source src="/src/assets/konig.mp3" type="audio/mpeg">
		</audio>
		<audio controls>
			<source src="/src/assets/gesang.ogg" type="audio/ogg">
		  	<source src="/src/assets/gesang.mp3" type="audio/mpeg">
		</audio>
		<audio controls>
			<source src="/src/assets/bozner.ogg" type="audio/ogg">
		  	<source src="/src/assets/bozner.mp3" type="audio/mpeg">
		</audio>
		<router-link :to="{ name: 'home' }" class="mt-5 hover:text-gray-200 dark:hover:text-gray-500 hover:underline">
			{{ $t('pages.home') }}
		</router-link>
	</div>
</template>

<style scoped></style>

<route lang="yaml">
name: other-page
</route>
