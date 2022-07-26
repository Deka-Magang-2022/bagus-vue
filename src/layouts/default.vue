<script setup lang="ts"></script>
<template>
	<header>
		<app-header />
	</header>

	<main
		class="
			
			dark:bg-gray-800 dark:text-white
			bg-white
			text-gray-800
			min-h-screen
			max-w-screen
		"
	>
		<router-view />
	</main>
</template>
