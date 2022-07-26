<script setup lang="ts">
	useHead({
		title: 'Daftar Doloe',
	});
</script>

<template>
	<div class="grid place-items-center w-full h-screen">
		<div class="w-full max-w-md">
			<form class="p-4 rounded-lg shadow-2xl dark:shadow-white dark:shadow-md">
				<div class="flex flex-col gap-5">
					<input class="form-control block w-full px-3 py-1.5 text-base font-normal text-gray-700 bg-white bg-clip-padding border border-solid border-gray-300 rounded transition ease-in-out m-0 shadow-md focus:text-gray-700 focus:bg-white focus:border-blue-600 focus:outline-none" placeholder="Username" type="text" name="username" id="username">
					<input class="form-control block w-full px-3 py-1.5 text-base font-normal text-gray-700 bg-white bg-clip-padding border border-solid border-gray-300 rounded transition ease-in-out m-0 shadow-md focus:text-gray-700 focus:bg-white focus:border-blue-600 focus:outline-none" placeholder="Password" type="password" name="password" id="password">
                    <input class="form-control block w-full px-3 py-1.5 text-base font-normal text-gray-700 bg-white bg-clip-padding border border-solid border-gray-300 rounded transition ease-in-out m-0 shadow-md focus:text-gray-700 focus:bg-white focus:border-blue-600 focus:outline-none" type="email" name="email" id="email" placeholder="E-mail">
				</div>
				<div class="text-center pt-1 mt-5 pb-1">
                    <a href="" class="inline-block px-6 py-2.5 dark:text-white dark:shadow-white dark:shadow-md text-gray-900 font-medium text-xs leading-tight uppercase rounded shadow-md hover:bg-blue-700 hover:shadow-lg hover:text-white focus:shadow-lg focus:outline-none focus:ring-0 active:shadow-lg transition duration-150 ease-in-out w-full mb-3" type="button">
					Buat
                    </a>
				</div>
			</form>
		</div>
	</div>
</template>

<route lang="yaml">
name: register
</route>