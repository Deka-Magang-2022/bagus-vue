<script setup lang="ts">
// defineEmits(["toggleSidebar"]);

const { availableLocales } = useI18n();

const preferedDark = usePreferredDark();
const isDark = useStorage("isDark", preferedDark.value);
const body = ref<HTMLBodyElement | null>(null);

const toggleDarkMode = () => {
  if (body.value) {
    if (isDark.value) {
      body.value.classList.remove("dark");
    } else {
      body.value.classList.add("dark");
    }
  }
  isDark.value = !isDark.value;
};

onMounted(async () => {
  await nextTick();

  body.value = document.querySelector("body") as HTMLBodyElement;
  if (body.value) {
    if (isDark.value) body.value.classList.add("dark");
  }
});
</script>

<template>
  <header>
    <nav
      class="w-full bg-white text-gray-800 dark:bg-gray-800 dark:text-white py-4 px-8 shadow-md dark:shadow-md flex items-center border-b border-gray-400/50"
    >
      <router-link :to="{ name: 'home' }">
        <div class="font-bold lg:text-xl md:text-lg text-md pr-1">Home</div>
      </router-link>
      <div class="">
        <router-link
          :to="{ name: 'formlogin' }"
          class="border-l-4 border-l-red-600 px-1 font-bold lg:text-xl md:text-lg text-md"
        >
          Log-in
        </router-link>
        <router-link
          :to="{ name: 'halaman' }"
          class="border-l-4 border-l-red-600 px-1 font-bold lg:text-xl md:text-lg text-md"
        >
          Halaman
        </router-link>
        <router-link
          :to="{ name: 'todo-list' }"
          class="border-l-4 border-l-red-600 px-1 font-bold lg:text-xl md:text-lg text-md"
        >
          Todo List
        </router-link>
        <router-link
          :to="{ name: 'kalkulator' }"
          class="border-l-4 border-l-red-600 px-1 font-bold lg:text-xl md:text-lg text-md"
        >
          Kalkulator
        </router-link>
        <router-link
          :to="{ name: 'netflix' }"
          class="border-l-4 border-l-red-600 px-1 font-bold lg:text-xl md:text-lg text-md"
        >
          Netflix Bootleg
        </router-link>
      </div>
      <div class="ml-auto flex items-center h-full">
        <select
          id="language"
          v-model="$i18n.locale"
          class="py-1 focus:outline-none rounded dark:text-gray-800"
        >
          <option v-for="locale in availableLocales" :key="locale" :value="locale">
            {{ locale }}
          </option>
        </select>
        <button class="mx-5 cursor-pointer focus:outline-none" @click="toggleDarkMode">
          <icon:bx:bx-moon class="w-6 h-6" v-if="!isDark" />
          <icon:bx:bxs-moon class="w-6 h-6" v-else />
        </button>
        <a href="https://github.com/knispel987">
          <icon-akar-icons:github-fill />
        </a>
      </div>
    </nav>
  </header>
</template>

<style scoped></style>
