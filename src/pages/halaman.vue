<script setup lang="ts">
	useHead({
		title: 'halaman desain',
	});
</script>

<template>
    <div class="relative grid bg-yellow-500">
		<p>grid 1</p>
    </div>
	<div>
		<router-link :to="{ name: 'home' }" class="mt-5 hover:text-gray-200 dark:hover:text-gray-500 hover:underline">
			{{ $t('pages.home') }}
		</router-link>
	</div>
</template>

<style scoped></style>

<route lang="yaml">
name: halaman
</route>
