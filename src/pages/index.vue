<script setup lang="ts">
	import { useStore } from '@/store';
	import VitailseLogo from '@/assets/logo.png';
	import Userimg from '@/assets/profil.png';
	import Markdown from '@/assets/markdown.md';
	useHead({
		title: 'poenya bagus',
	});

	const store = useStore();
	const { t } = useI18n();
</script>

<template>
	<div class="grid place-items-center min-h-[80vh]">
		<div class="grid bg-emerald-400 border-4 border-red-600 text-stone-900 dark:bg-green-600/40 px-10 py-10 shadow-2x1 dark:shadow-sky-500 rounded w-full max-w-2xl dark:border-teal-400 text-center place-items-center dark:text-white ouline outline-dark-900 min-h-[80vh]">
			<h1 class="uppercase font-bold text-xl mt-10">profil</h1>
			<img :src="Userimg" width="300" class="rounded-full	mx-auto" />
			<div class="text-sm text-left">
				<p> Nama : Bagus </p>
				<p> Date Of Birth : 2005-9-8</p>
				<p> Religion : Islam </p>
				<p> Gender : L </p>
			</div>
			<div class="grid max-w-lg text-center place-items-center mt-10">
				<h1 class="uppercase font-bold text-xl">Contact</h1>
				<div class="text-sm text-justify ">
					<p> Email : <a href="mailto:knispel1999@gmail.com" target="_blank" class="after:content-['_↗'] text-purple-600 dark:hover:text-sky-200 font-bold">knispel1999@gmail.com</a></p>
					<a href="https://github.com/knispel987" target="_blank"
						class="after:content-['_↗'] text-purple-600 dark:hover:text-sky-200 font-bold">Github</a>
				</div>
			</div>
			<div class="max-w-lg py-10 text-center mt-10">
				<h1 class="uppercase font-bold text-xl">About</h1>
				<p class="text-sm text-justify"> hallo, mein name ist bagus, ich weisse nicht wer ich bin </p>
			</div>
			<div class="max-w-2xl w-full grid grid-flow-row grid-cols-3 gap-5 mt-10 px-4 py-3">
				<a href="todo-list" class="bg-gray-500 rounded-sm hover:bg-gray-900 hover:text-white">Halaman Todo List</a>
				<a href="kalkulator" class="bg-gray-500 rounded-sm hover:bg-gray-900 hover:text-white">Kalkulator</a>
				<a href="jurnal" class="bg-gray-500 rounded-sm hover:bg-gray-900 hover:text-white">Jurnal</a>
			</div>
		</div>
	</div>
</template>

<route lang="yaml">
name: home
</route>
