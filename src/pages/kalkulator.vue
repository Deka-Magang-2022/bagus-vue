<script setup lang="ts">
useHead({
	title: 'kalkulator',
});

import { useStore } from '@/store';

const store = useStore();
let tempType = '';
store.temp = '';
store.input = '';

const operators = {
	'/': '/',
	'X': 'X',
	'-': '-',
	'+': '+',
	'=': '=',
}

const addNumber = (number: any) => {
	store.input += number
}

const calculate = (operator: string) => {
	if (operator !== '=') {
		store.input += operator
	} else {
		try {
				store.temp = eval(store.input.replace(/X/g, '*'))
		} catch (error) {
			store.temp = 'Error'
		}
	}
}

const clear = () => {
	store.input = ''
	store.temp = ''
}

const removeLast = () => {
	store.input = store.input.slice(0, -1);
}
</script>
<template>
	<div class="min-h-[80vh]">
		<div class="max-w-lg mb-10 border border-gray-700 rounded-md p-5 dark:bg-gray-800">
			<div class="w-full">
				<p>Hasil :</p>
				<div class="flex justify-end px-4 py-2 dark:text-white border-b-4 mb-6 border-b-blue-900 border-r-4 border-r-blue-900 dark:border-r dark:border-b dark:border-b-gray-400 dark:border-r-gray-300"
					:class="{ 'bg-red-500 rounded-md text-white dark:text-gray-900': store.temp == 'Error' }">
					{{ store.temp }}
				</div>
				<input disabled class="w-full bg-gray-200 rounded-md px-4 py-2 text-right dark:bg-black dark:text-white" type="text" v-model="store.input">
			</div>
			<div class="w-full grid grid-flow-row grid-cols-4 mt-5 gap-5">
				<div class="w-full grid grid-flow-row grid-cols-3 gap-5 col-span-3 dark:text-white">
					<button @click="clear()" type="button"
						class="border border-gray-700 p-4 bg-gray-100 rounded-md col-span-2 dark:bg-black active:bg-green-200">
						Clear
					</button>
					<button @click="removeLast()" type="button"
						class="border border-gray-700 p-4 bg-gray-100 rounded-md dark:bg-black flex items-center justify-center active:bg-green-200">
						<icon-akar-icons:backspace class="w-6 h-6" />
					</button>
					<button @click="addNumber(number)" type="button"
						class="border border-gray-700 p-4 bg-gray-100 rounded-md dark:bg-black active:bg-green-200" v-for="(number) in 9" :key="number">
						{{ number }}
					</button>
					<button @click="addNumber(0)" type="button"
						class="active:bg-green-200 border border-gray-700 p-4 bg-gray-100 dark:bg-black rounded-md col-span-3">
						0
					</button>
				</div>
				<div class="w-full grid grid-flow-row gap-5">
					<button @click="calculate(operator)" type="button"
						class="border border-gray-700 p-4 bg-gray-100 rounded-md dark:bg-black active:bg-green-200" v-for="(type, operator) in operators"
						:key="operator">
						{{ type }}
					</button>
				</div>
			</div>
		</div>
	</div>
</template>

<style scoped>
</style>

<route lang="yaml">
name: kalkulator
</route>