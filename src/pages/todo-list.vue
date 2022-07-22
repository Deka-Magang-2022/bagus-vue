<script setup lang="ts">
import { useStore } from '@/store';
const store = useStore();
let variabelInput = '';
	useHead({
		title: 'todo list',
	});
	store.listTodo = [];
	const simpanData = (value) =>{
		store.listTodo.push(value)
	}
	const hapusData = (value) => {
	store.listTodo.splice( value, 1)
	}
</script>

<template>
	<div>
		<div class="min-h[70vh]">
			<h1 class="text-xl">Halaman Todo List</h1>
			<div class="flex">
				<input v-model="variabelInput" class="w-full rounded-lg mr-2 dark:text-gray-900"
					type="text">
				<button @click="simpanData(variabelInput)" type="button"
					class="px-4 py-2 bg-indigo-300 rounded-lg active:bg-indigo-600">Add</button>
			</div>
			<div class="grid grid-cols-2">
				<div class="grid bg-green-300" v-for="(item, index) in store.listTodo" :key="index">
					{{ item }}
					<button class="bg-red-500 m-9" @click="hapusData(index)" type="button">
					Hapus	
					</button>
				</div>
			</div>
		</div>
		<router-link :to="{ name: 'home' }" class="mt-5 hover:text-blue-200 dark:hover:text-gray-500 hover:underline">{{ $t('pages.home') }}</router-link>
	</div>
</template>

<style scoped></style>

<route lang="yaml">
name: todo-list
</route>
