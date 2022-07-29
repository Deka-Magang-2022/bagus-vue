<script setup lang="ts">
	useHead({
		title: 'halaman',
	});
</script>

<template>
    <div class="w-full flex flex-col place-items-center">
         <div class="grid grid-cols-6 h-screen w-full">
            <div class="col-span-4 bg-yellow-400">
            </div>
            <div class="col-span-2 bg-rose-600 grid grid-rows-5">
                <div class="row-span-2"></div>
                <div class="row-span-3 grid grid-rows-3 grid-cols-3">
                    <div class="bg-cyan-500"></div>
                    <div class="bg-yellow-500"></div>
                    <div class="bg-blue-500"></div>
                    <div class="bg-purple-500"></div>
                    <div class="bg-green-500"></div>
                    <div class="bg-lime-500"></div>
                    <div class="bg-indigo-500"></div>
                    <div class="bg-pink-500"></div>
                    <div class="bg-emerald-500"></div>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped></style>

<route lang="yaml">
name: halaman
</route>
