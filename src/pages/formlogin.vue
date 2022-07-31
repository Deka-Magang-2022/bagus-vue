<script setup lang="ts">
import photo from "@/assets/erwin.jpg";
useHead({
  title: "Log-in",
});
</script>

<template>
  <div
    class="flex flex-col place-items-center w-full h-screen justify-evenly bg-no-repeat bg-cover bg-[url(https://deka.dev/images/ilustration-1.png)] dark:bg-gray-800"
  >
    <section class="w-full h-full backdrop-blur-xl flex place-content-center">
      <div class="w-full max-w-4xl">
        <form class="p-4 rounded-lg">
          <div class="flex flex-col backdrop-blur-xl bg-gray-700/20 p-5">
            <section class="flex flex-row">
              <svg
                class="w-10 h-auto"
                xmlns="http://www.w3.org/2000/svg"
                aria-hidden="true"
                role="img"
                width="1em"
                height="1em"
                preserveAspectRatio="xMidYMid meet"
                viewBox="0 0 48 48"
              >
                <g fill="currentColor" fill-rule="evenodd" clip-rule="evenodd">
                  <path
                    d="M14.809 34.714c6.845-1 11.558-.914 18.412.035A2.077 2.077 0 0 1 35 36.818c0 .48-.165.946-.463 1.31A61.165 61.165 0 0 1 32.941 40h2.641c.166-.198.333-.4.502-.605A4.071 4.071 0 0 0 37 36.819c0-2.025-1.478-3.77-3.505-4.05c-7.016-.971-11.92-1.064-18.975-.033c-2.048.299-3.52 2.071-3.52 4.11c0 .905.295 1.8.854 2.525c.165.214.328.424.49.63h2.577a57.88 57.88 0 0 1-1.482-1.85A2.144 2.144 0 0 1 13 36.845c0-1.077.774-1.98 1.809-2.131ZM24 25a6 6 0 1 0 0-12a6 6 0 0 0 0 12Zm0 2a8 8 0 1 0 0-16a8 8 0 0 0 0 16Z"
                  />
                  <path
                    d="M24 42c9.941 0 18-8.059 18-18S33.941 6 24 6S6 14.059 6 24s8.059 18 18 18Zm0 2c11.046 0 20-8.954 20-20S35.046 4 24 4S4 12.954 4 24s8.954 20 20 20Z"
                  />
                </g>
              </svg>
              <input
                class="form-control block text-gray-700 bg-transparent border-transparent transition ease-in-out m-0 placeholder-white w-full focus:outline-none focus:border-transparent focus:ring-0 focus:border-b-slate-800"
                placeholder="Username"
                type="text"
                name="username"
                id="username"
              />
            </section>
            <section class="flex flex-row">
              <svg
                class="w-10 h-auto"
                xmlns="http://www.w3.org/2000/svg"
                aria-hidden="true"
                role="img"
                width="1em"
                height="1em"
                preserveAspectRatio="xMidYMid meet"
                viewBox="0 0 1024 1024"
              >
                <path
                  fill="currentColor"
                  d="M832 464h-68V240c0-70.7-57.3-128-128-128H388c-70.7 0-128 57.3-128 128v224h-68c-17.7 0-32 14.3-32 32v384c0 17.7 14.3 32 32 32h640c17.7 0 32-14.3 32-32V496c0-17.7-14.3-32-32-32zM332 240c0-30.9 25.1-56 56-56h248c30.9 0 56 25.1 56 56v224H332V240zm460 600H232V536h560v304zM484 701v53c0 4.4 3.6 8 8 8h40c4.4 0 8-3.6 8-8v-53a48.01 48.01 0 1 0-56 0z"
                />
              </svg>
              <input
                class="form-control block text-gray-700 bg-transparent border-transparent transition ease-in-out m-0 placeholder-white w-full focus:outline-none focus:border-transparent focus:ring-0 focus:border-b-slate-800"
                placeholder="Password"
                type="password"
                name="password"
                id="password"
              />
            </section>
          </div>
          <div class="flex place-content-center text-center mt-5">
            <a
              href=""
              class="bg-gray-200 py-2 w-full max-w-sm focus:shadow-lg focus:outline-none focus:ring-0 active:shadow-lg transition duration-150 ease-in-out mb-3"
              type="button"
            >
              Masuk
            </a>
          </div>
          <div class="text-center">
            <a class="text-blue-500 hover:underline" href="">Lupa Password?</a>
          </div>
          <div
            class="flex items-center my-4 before:flex-1 before:border-t before:border-gray-900 before:mt-0.5 after:flex-1 after:border-t after:border-gray-900 after:mt-0.5"
          >
            <p class="text-center font-semibold mx-4 mb-0">Atau</p>
          </div>
          <div class="text-center">
            <a
              href="register"
              class="inline-block py-3 dark:text-white bg-blue-500 text-gray-900 font-medium text-xs leading-tight uppercase rounded shadow-md hover:bg-blue-700 hover:shadow-lg hover:text-white focus:shadow-lg focus:outline-none focus:ring-0 active:shadow-lg transition duration-150 ease-in-out w-40 max-w-md mb-3"
              type="button"
            >
              Buat Akun Baru ?
            </a>
          </div>
        </form>
      </div>
    </section>
  </div>
</template>

<style scoped></style>

<route lang="yaml">
name: formlogin
</route>
