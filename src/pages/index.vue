<script setup lang="ts">
	import Userimg from '@/assets/profil.jpg';
	useHead({
		title: 'poenya bagus',
	});
</script>

<template>
	<div class="grid place-items-center min-h-[80vh]">
		<div class="grid bg-gray-200 px-10 pt-5 shadow-2xl dark:shadow-white dark:shadow-lg dark:bg-gray-900 rounded-lg">
			<h1 class="uppercase font-bold text-xl text-center">profil</h1>
			<img :src="Userimg" width="300" class="dark:shadow-white dark:shadow-md rounded-full mx-auto animate-pulse"/>
			<div class="grid place-content-center text-justify text-sm mt-6">
				<p> Name          : Bagus </p>
				<p> Geburtsdatum  : 2005-9-8</p>
				<p> Religion      : Islam </p>
				<p> Geschlect     : L </p>
			</div>
			<div class="grid max-w-lg text-center place-items-center mt-10">
				<h1 class="uppercase font-bold text-xl">Kontakt</h1>
				<div class="text-sm text-justify">
					<p> Email : <a href="mailto:knispel1999@gmail.com" target="_blank" class="after:content-['_↗'] text-purple-600 dark:hover:text-sky-200 font-bold">
					knispel1999@gmail.com
					</a></p>
					<a href="https://github.com/knispel987" target="_blank" class="after:content-['_↗'] text-purple-600 dark:hover:text-sky-200 font-bold">
					Github
					</a>
				</div>
			</div>
			<div class="max-w-lg py-10 text-center mt-10">
				<h1 class="uppercase font-bold text-xl">Uber Mich</h1>
				<p class="text-sm text-justify">
					hallo, mein name ist bagus, ich weisse nicht wer ich bin 
				</p>
			</div>
		</div>
	</div>
</template>

<route lang="yaml">
name: home
</route>
