<script setup lang="ts">
// import photo from "@/assets/bangerwin.jfif";
useHead({
  title: "Log-in",
});
</script>

<template>
  <div class="grid place-items-center w-full h-screen grid-cols-2">
    <div>
      <img :src="photo" alt="foto" class="w-screen pl-7" />
    </div>
    <div class="w-full max-w-sm">
      <form class="p-4 rounded-lg shadow-2xl dark:shadow-white dark:shadow-md">
        <div class="flex flex-col gap-5">
          <input
            class="form-control block w-full px-3 py-1.5 text-base font-normal text-gray-700 bg-white bg-clip-padding border border-solid border-gray-300 rounded transition ease-in-out m-0 shadow-md focus:text-gray-700 focus:bg-white focus:border-blue-600 focus:outline-none"
            placeholder="Username Anda"
            type="text"
            name="username"
            id="username"
          />
          <input
            class="form-control block w-full px-3 py-1.5 text-base font-normal text-gray-700 bg-white bg-clip-padding border border-solid border-gray-300 rounded transition ease-in-out m-0 shadow-md focus:text-gray-700 focus:bg-white focus:border-blue-600 focus:outline-none"
            placeholder="Password Anda"
            type="password"
            name="password"
            id="password"
          />
        </div>
        <div class="text-center pt-1 mt-5 pb-1">
          <a
            href=""
            class="inline-block px-6 py-2.5 dark:text-white dark:shadow-white dark:shadow-md text-gray-900 font-medium text-xs leading-tight uppercase rounded shadow-md hover:bg-blue-700 hover:shadow-lg hover:text-white focus:shadow-lg focus:outline-none focus:ring-0 active:shadow-lg transition duration-150 ease-in-out w-full mb-3"
            type="button"
          >
            Log-in
          </a>
        </div>
        <div class="text-center">
          <a class="text-blue-500 hover:underline" href="">Lupa Password?</a>
        </div>
        <div
          class="flex items-center my-4 before:flex-1 before:border-t before:border-gray-300 before:mt-0.5 after:flex-1 after:border-t after:border-gray-300 after:mt-0.5"
        >
          <p class="text-center font-semibold mx-4 mb-0">Atau</p>
        </div>
        <div class="text-center">
          <a
            href="register"
            class="inline-block py-3 dark:text-white bg-green-500 text-gray-900 font-medium text-xs leading-tight uppercase rounded shadow-md hover:bg-green-700 hover:shadow-lg hover:text-white focus:shadow-lg focus:outline-none focus:ring-0 active:shadow-lg transition duration-150 ease-in-out w-full mb-3"
            type="button"
          >
            Buat Akun Baru
          </a>
        </div>
      </form>
    </div>
  </div>
</template>

<style scoped></style>

<route lang="yaml">
name: formlogin
</route>
