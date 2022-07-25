<script setup lang="ts">
import JurnalMd from '@/assets/jurnal.md';
	useHead({
		title: 'Jurnal',
	});
</script>

<template>
	<div>
		<JurnalMd />
		<router-link :to="{ name: 'home' }" class="mt-5 hover:text-gray-200 dark:hover:text-gray-500 hover:underline">
			{{ $t('pages.home') }}
		</router-link>
	</div>
</template>

<style scoped></style>

<route lang="yaml">
name: jurnal
</route>