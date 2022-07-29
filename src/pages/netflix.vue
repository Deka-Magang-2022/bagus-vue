<script setup lang="ts">
import Icon from "@/assets/plus.png";

useHead({
  title: "Netflix",
});
</script>

<template>
  <div class="text-white">
    <section>
      <div
        class="bg-cover"
        style="
          background-image: url('https://assets.nflxext.com/ffe/siteui/vlv3/c2578c37-8569-4f88-b8f1-67a26a9ddcdd/2e83f3ab-d9d1-4f3a-81cb-2bb62aee8b5f/ID-en-20220725-popsignuptwoweeks-perspective_alpha_website_large.jpg');
        "
      >
        <div
          class="bg-gradient-to-b from-black via-black/20 to-black border-b-[9px] border-b-gray-800"
        >
          <div class="grid w-full h-screen place-content-center">
            <section class="w-full absolute">
              <nav class="place-items-start p-10 flex">
                <p class="text-5xl text-red-500 uppercase">Netflix</p>
                <div class="ml-auto space-x-4">
                  <select name="languange" id="language" class="bg-transparent">
                    <option value="en">English</option>
                  </select>
                  <button class="bg-red-600 px-4 py-2" href="">Masuk</button>
                </div>
              </nav>
            </section>
            <section class="text-white text-7xl font-medium text-center font-[arial]">
              <h1>
                Unlimited movies, TV<br />
                shows, and more.
              </h1>
              <p class="text-3xl pt-[35px]">Watch anywhere, Cancel anytime</p>
              <p class="text-lg pt-[45px]">
                Ready to watch? Enter your email to create or restart your membership.
              </p>
            </section>
            <section class="flex flex-row">
              <input
                type="email"
                name="email"
                id="email"
                placeholder="Alamat E-mail"
                class="text-black w-[500px] h-[68px]"
              />
              <button class="bg-red-600 text-white px-5 py-2 text-3xl" type="submit">
                Get Started >
              </button>
            </section>
          </div>
        </div>
      </div>
    </section>
  </div>
  <div class="grid gap-2 bg-gray-800 text-white">
    <section class="flex justify-between bg-black h-[527px]">
      <section class="ml-40 mt-40 place-content-center">
        <p class="text-5xl mb-9">Enjoy on your TV.<br /></p>
        <p class="text-2xl mt-4">
          Watch on Smart TVs, Playstation, Xbox,<br />
          Chromecast, Apple TV, Blu-ray players, and <br />
          more.
        </p>
      </section>
      <img
        class="mr-48 w-[400px] h-96 mt-20"
        src="https://assets.nflxext.com/ffe/siteui/acquisition/ourStory/fuji/desktop/tv.png"
        alt=""
        srcset=""
      />
    </section>
    <section class="flex justify-between bg-black h-[527px]">
      <img
        class="w-[400] h-96 mt-20 ml-20"
        src="https://assets.nflxext.com/ffe/siteui/acquisition/ourStory/fuji/desktop/mobile-0819.jpg"
        alt=""
      />
      <section class="mr-40 mt-40 place-content-center">
        <p class="text-5xl mb-9">Download your shows <br />to watch offline.</p>
        <p class="text-2xl mt-4">
          Save your favorites easily and always have<br />
          something to watch. <br />
        </p>
      </section>
    </section>
    <section class="flex justify-between bg-black h-[527px]">
      <section class="ml-40 mt-40 place-content-center">
        <p class="text-5xl mb-9">Watch everywhere.<br /></p>
        <p class="text-2xl mt-4">
          Stream unlimited movies and TV shows on<br />your phone, tablet, laptop, and TV.
          <br />
          more.
        </p>
      </section>
      <img
        src="https://assets.nflxext.com/ffe/siteui/acquisition/ourStory/fuji/desktop/device-pile-id.png"
      />
    </section>
    <section class="flex justify-between bg-black h-[500px]">
      <img
        class="w-auto h-[400px] mt-10 mr-10"
        src="https://occ-0-64-58.1.nflxso.net/dnm/api/v6/19OhWN2dO19C9txTON9tvTFtefw/AAAABfpnX3dbgjZ-Je8Ax3xn0kXehZm_5L6-xe6YSTq_ucht9TI5jwDMqusWZKNYT8DfGudD0_wWVVTFLiN2_kaQJumz2iivUWbIbAtF.png?r=11f"
      />
      <section class="mr-40 mt-40 place-content-center">
        <p class="text-5xl mb-9">Create profiles for kids.<br /></p>
        <p class="text-2xl mt-4">
          Send kids on adventures with their favorite<br />characters in a space made just
          for them—<br />free with your membership.
        </p>
      </section>
    </section>
    <section class="text-center bg-black h-[975px]">
      <h1 class="text-5xl font-semibold mt-16">Frequently Asked Questions</h1>
      <section class="text-left flex place-content-center">
        <div class="text-3xl flex flex-col gap-2 mt-6">
          <section
            class="bg-gray-700 w-[890px] h-[80px] p-6 flex flex-row justify-between"
          >
            <button>What is Netflix?</button>
            <div>
              <svg
                class="w-[35px] h-auto"
                xmlns="http://www.w3.org/2000/svg"
                xmlns:xlink="http://www.w3.org/1999/xlink"
                aria-hidden="true"
                role="img"
                id="footer-sample-full"
                preserveAspectRatio="xMidYMid meet"
                viewBox="0 0 24 24"
              >
                <path
                  fill="none"
                  stroke="currentColor"
                  stroke-linecap="round"
                  stroke-width="2"
                  d="M12 20v-8m0 0V4m0 8h8m-8 0H4"
                ></path>
              </svg>
            </div>
          </section>
          <section
            class="bg-gray-700 w-[890px] h-[80px] p-6 flex flex-row justify-between"
          >
            <button>How much does Netflix cost?</button>
            <div>
              <svg
                class="w-[35px] h-auto"
                xmlns="http://www.w3.org/2000/svg"
                xmlns:xlink="http://www.w3.org/1999/xlink"
                aria-hidden="true"
                role="img"
                id="footer-sample-full"
                preserveAspectRatio="xMidYMid meet"
                viewBox="0 0 24 24"
              >
                <path
                  fill="none"
                  stroke="currentColor"
                  stroke-linecap="round"
                  stroke-width="2"
                  d="M12 20v-8m0 0V4m0 8h8m-8 0H4"
                ></path>
              </svg>
            </div>
          </section>
          <section
            class="bg-gray-700 w-[890px] h-[80px] p-6 flex flex-row justify-between"
          >
            <button>Where can I watch?</button>
            <div>
              <svg
                class="w-[35px] h-auto"
                xmlns="http://www.w3.org/2000/svg"
                xmlns:xlink="http://www.w3.org/1999/xlink"
                aria-hidden="true"
                role="img"
                id="footer-sample-full"
                preserveAspectRatio="xMidYMid meet"
                viewBox="0 0 24 24"
              >
                <path
                  fill="none"
                  stroke="currentColor"
                  stroke-linecap="round"
                  stroke-width="2"
                  d="M12 20v-8m0 0V4m0 8h8m-8 0H4"
                ></path>
              </svg>
            </div>
          </section>
          <section
            class="bg-gray-700 w-[890px] h-[80px] p-6 flex flex-row justify-between"
          >
            <button>How do I cancel?</button>
            <div>
              <svg
                class="w-[35px] h-auto"
                xmlns="http://www.w3.org/2000/svg"
                xmlns:xlink="http://www.w3.org/1999/xlink"
                aria-hidden="true"
                role="img"
                id="footer-sample-full"
                preserveAspectRatio="xMidYMid meet"
                viewBox="0 0 24 24"
              >
                <path
                  fill="none"
                  stroke="currentColor"
                  stroke-linecap="round"
                  stroke-width="2"
                  d="M12 20v-8m0 0V4m0 8h8m-8 0H4"
                ></path>
              </svg>
            </div>
          </section>
          <section
            class="bg-gray-700 w-[890px] h-[80px] p-6 flex flex-row justify-between"
          >
            <button>What can I watch on Netflix?</button>
            <div>
              <svg
                class="w-[35px] h-auto"
                xmlns="http://www.w3.org/2000/svg"
                xmlns:xlink="http://www.w3.org/1999/xlink"
                aria-hidden="true"
                role="img"
                id="footer-sample-full"
                preserveAspectRatio="xMidYMid meet"
                viewBox="0 0 24 24"
              >
                <path
                  fill="none"
                  stroke="currentColor"
                  stroke-linecap="round"
                  stroke-width="2"
                  d="M12 20v-8m0 0V4m0 8h8m-8 0H4"
                ></path>
              </svg>
            </div>
          </section>
          <section
            class="bg-gray-700 w-[890px] h-[80px] p-6 flex flex-row justify-between"
          >
            <button>Is Netflix good for kids?</button>
            <div>
              <svg
                class="w-[35px] h-auto"
                xmlns="http://www.w3.org/2000/svg"
                xmlns:xlink="http://www.w3.org/1999/xlink"
                aria-hidden="true"
                role="img"
                id="footer-sample-full"
                preserveAspectRatio="xMidYMid meet"
                viewBox="0 0 24 24"
              >
                <path
                  fill="none"
                  stroke="currentColor"
                  stroke-linecap="round"
                  stroke-width="2"
                  d="M12 20v-8m0 0V4m0 8h8m-8 0H4"
                ></path>
              </svg>
            </div>
          </section>
        </div>
      </section>
      <p class="text-lg pt-[70px]">
        Ready to watch? Enter your email to create or restart your membership.
      </p>
      <section class="mt-8 flex flex-row place-content-center">
        <input
          type="email"
          name="email"
          id="email"
          placeholder="Alamat E-mail"
          class="text-black w-[500px] h-[68px]"
        />
        <button class="bg-red-600 text-white px-5 py-2 text-3xl" type="submit">
          Get Started >
        </button>
      </section>
    </section>
    <section class="bg-black h-[450px] px-60 py-10 text-gray-600">
      <p class="pb-4">
        Questions? Call <a class="hover:underline" href="">007-803-321-2130</a>
      </p>
      <div class="grid grid-cols-4 grid-rows-4 gap-5">
        <a class="hover:underline" href="">FAQ</a>
        <a class="hover:underline" href="">Help Center</a>
        <a class="hover:underline" href="">Account</a>
        <a class="hover:underline" href="">Media Center</a>
        <a class="hover:underline" href="">Investor Relations</a>
        <a class="hover:underline" href="">Jobs</a>
        <a class="hover:underline" href="">Redeem Gift Cards</a>
        <a class="hover:underline" href="">Buy Gift Cards</a>
        <a class="hover:underline" href="">Ways to Watch</a>
        <a class="hover:underline" href="">Terms of Use</a>
        <a class="hover:underline" href="">Privacy</a>
        <a class="hover:underline" href="">Cookie Preferences</a>
        <a class="hover:underline" href="">Corporate Information</a>
        <a class="hover:underline" href="">Contact Us</a>
        <a class="hover:underline" href="">Speed Test</a>
        <a class="hover:underline" href="">Legal Notices</a>
        <a class="hover:underline" href="">Only on Netflix</a>
      </div>
      <div class="mt-9">
        <select name="languange" id="language" class="bg-transparent">
          <option value="en">English</option>
        </select>
        <p class="text-xs mt-4">Netflix Bootleg Edition</p>
      </div>
    </section>
  </div>
</template>

<style scoped></style>

<route lang="yaml">
name: netflix
</route>
