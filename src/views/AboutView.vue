<template>
  <section class="movie-time">
    <div class="discover-base"></div>
    <div class="mx-7 lg:mx-6 mt-32 flex-grow">
      <div class="max-w-6xl mx-auto">
        <div class="rectangle"></div>
        <h1 class="text-3xl leading-normal font-bold mt-0 mb-7 label-discover pt-4">
          Movies
        </h1>
        <div class="grid grid-cols-4 gap-1 justify-evenly">
          <div class="d-filter">
            <p class="text-1">Sort Result By</p>
            <div class="dropdown-filter">
              <div class="relative text-lg w-48">
                <button
                  class="flex items-center justify-between px-3 py-2 text-white w-full"
                  @click="isOptionsExpanded = !isOptionsExpanded"
                  @blur="isOptionsExpanded = false"
                >
                  <span>{{ selectedOption }}</span>
                  <svg
                    fill="none"
                    viewBox="0 0 24 24"
                    stroke="currentColor"
                    class="h-4 w-4 transform transition-transform duration-200 ease-in-out"
                    :class="isOptionsExpanded ? 'rotate-180' : 'rotate-0'"
                  >
                    <path
                      stroke-linecap="round"
                      stroke-linejoin="round"
                      stroke-width="2"
                      d="M19 9l-7 7-7-7"
                    />
                  </svg>
                </button>
                <transition
                  enter-active-class="transform transition duration-500 ease-custom"
                  enter-class="-translate-y-1/2 scale-y-0 opacity-0"
                  enter-to-class="translate-y-0 scale-y-100 opacity-100"
                  leave-active-class="transform transition duration-300 ease-custom"
                  leave-class="translate-y-0 scale-y-100 opacity-100"
                  leave-to-class="-translate-y-1/2 scale-y-0 opacity-0"
                >
                  <ul
                    v-show="isOptionsExpanded"
                    class="absolute left-0 right-0 mb-4 bg-white divide-y overflow-hidden u-dropdown-filter"
                  >
                    <li
                      v-for="(option, index) in options"
                      :key="index"
                      class="px-3 py-2 transition-colors duration-300 hover:bg-gray-200"
                      @mousedown.prevent="setOption(option)"
                    >
                      {{ option }}
                    </li>
                  </ul>
                </transition>
              </div>
            </div>
            <div class="genred-box">
              <h2>Genre</h2>
            </div>
            <div class="box-check">
              <div class="flex items-center">
                <label
                  for="bordered-checkbox-1"
                  class="w-full py-4 ml-2 text-sm font-medium text-gray-900 dark:text-gray-300"
                  >Action</label
                >
                <input
                  id="bordered-checkbox-1"
                  type="checkbox"
                  value=""
                  name="bordered-checkbox"
                  class="w-4 h-4 text-blue-600 focus:ring-blue-500 dark:focus:ring-blue-600 dark:ring-offset-gray-800 focus:ring-2"
                />
              </div>
              <div class="flex items-center">
                <label
                  for="bordered-checkbox-1"
                  class="w-full py-4 ml-2 text-sm font-medium text-gray-900 dark:text-gray-300"
                  >Adventure</label
                >
                <input
                  id="bordered-checkbox-1"
                  type="checkbox"
                  value=""
                  name="bordered-checkbox"
                  class="w-4 h-4 text-blue-600 focus:ring-blue-500 dark:focus:ring-blue-600 dark:ring-offset-gray-800 focus:ring-2"
                />
              </div>
              <div class="flex items-center">
                <label
                  for="bordered-checkbox-1"
                  class="w-full py-4 ml-2 text-sm font-medium text-gray-900 dark:text-gray-300"
                  >Animation</label
                >
                <input
                  id="bordered-checkbox-1"
                  type="checkbox"
                  value=""
                  name="bordered-checkbox"
                  class="w-4 h-4 text-blue-600 focus:ring-blue-500 dark:focus:ring-blue-600 dark:ring-offset-gray-800 focus:ring-2"
                />
              </div>
              <div class="flex items-center">
                <label
                  for="bordered-checkbox-1"
                  class="w-full py-4 ml-2 text-sm font-medium text-gray-900 dark:text-gray-300"
                  >Comedy</label
                >
                <input
                  id="bordered-checkbox-1"
                  type="checkbox"
                  value=""
                  name="bordered-checkbox"
                  class="w-4 h-4 text-blue-600 focus:ring-blue-500 dark:focus:ring-blue-600 dark:ring-offset-gray-800 focus:ring-2"
                />
              </div>
              <div class="flex items-center">
                <label
                  for="bordered-checkbox-1"
                  class="w-full py-4 ml-2 text-sm font-medium text-gray-900 dark:text-gray-300"
                  >Crime</label
                >
                <input
                  id="bordered-checkbox-1"
                  type="checkbox"
                  value=""
                  name="bordered-checkbox"
                  class="w-4 h-4 text-blue-600 focus:ring-blue-500 dark:focus:ring-blue-600 dark:ring-offset-gray-800 focus:ring-2"
                />
              </div>
              <div class="flex items-center">
                <label
                  for="bordered-checkbox-1"
                  class="w-full py-4 ml-2 text-sm font-medium text-gray-900 dark:text-gray-300"
                  >Documentary</label
                >
                <input
                  id="bordered-checkbox-1"
                  type="checkbox"
                  value=""
                  name="bordered-checkbox"
                  class="w-4 h-4 text-blue-600 focus:ring-blue-500 dark:focus:ring-blue-600 dark:ring-offset-gray-800 focus:ring-2"
                />
              </div>
              <div class="flex items-center">
                <label
                  for="bordered-checkbox-1"
                  class="w-full py-4 ml-2 text-sm font-medium text-gray-900 dark:text-gray-300"
                  >Drama</label
                >
                <input
                  id="bordered-checkbox-1"
                  type="checkbox"
                  value=""
                  name="bordered-checkbox"
                  class="w-4 h-4 text-blue-600 focus:ring-blue-500 dark:focus:ring-blue-600 dark:ring-offset-gray-800 focus:ring-2"
                />
              </div>
              <div class="flex items-center">
                <label
                  for="bordered-checkbox-1"
                  class="w-full py-4 ml-2 text-sm font-medium text-gray-900 dark:text-gray-300"
                  >Family</label
                >
                <input
                  id="bordered-checkbox-1"
                  type="checkbox"
                  value=""
                  name="bordered-checkbox"
                  class="w-4 h-4 text-blue-600 focus:ring-blue-500 dark:focus:ring-blue-600 dark:ring-offset-gray-800 focus:ring-2"
                />
              </div>
            </div>
          </div>
          <!-- wrap column -->
          <div class="col-start-2 col-span-3 flex flex-wrap">
            <div class="w-full sm:w-1/2 md:w-1/4 self-stretch p-2 mb-2 static">
              <div class="absolute w-192">
                <p class="right-0 relative bx-ractangle">7.0</p>
              </div>
              <div class="rounded shadow-md h-full box-card">
                <router-link to="/detail"
                  ><img
                    class="w-full m-0 rounded-t lazy"
                    src="../assets/movies-1.png"
                    alt="This post thumbnail"
                    width="960"
                    height="500"
                /></router-link>

                <div class="px-0 py-5">
                  <div class="font-semibold text-lg mb-2">
                    <router-link class="text-slate-900 hover:text-slate-700" to="/detail"
                      >Wonder Women 1994</router-link
                    >
                  </div>
                  <p class="text-slate-700 mb-1" title="Published date">2020</p>
                </div>
              </div>
            </div>
            <div class="w-full sm:w-1/2 md:w-1/4 self-stretch p-2 mb-2 static">
              <div class="absolute w-192">
                <p class="right-0 relative bx-ractangle">64</p>
              </div>
              <div class="rounded shadow-md h-full box-card">
                <router-link to="/detail"
                  ><img
                    class="w-full m-0 rounded-t lazy"
                    src="../assets/movies-2.png"
                    alt="This post thumbnail"
                    width="960"
                    height="500"
                /></router-link>
                <div class="px-0 py-5">
                  <div class="font-semibold text-lg mb-2">
                    <router-link class="text-slate-900 hover:text-slate-700" to="/detail"
                      >Below Zero</router-link
                    >
                  </div>
                  <p class="text-slate-700 mb-1" title="Published date">2021</p>
                </div>
              </div>
            </div>
            <div class="w-full sm:w-1/2 md:w-1/4 self-stretch p-2 mb-2 static">
              <div class="absolute w-192">
                <p class="right-0 relative bx-ractangle">6.4</p>
              </div>
              <div class="rounded shadow-md h-full box-card">
                <router-link to="/detail"
                  ><img
                    class="w-full m-0 rounded-t lazy"
                    src="../assets/movies-3.png"
                    alt="This post thumbnail"
                    width="960"
                    height="500"
                /></router-link>
                <div class="px-0 py-5">
                  <div class="font-semibold text-lg mb-2">
                    <router-link class="text-slate-900 hover:text-slate-700" to="/detail"
                      >The Little Things</router-link
                    >
                  </div>
                  <p class="text-slate-700 mb-1" title="Published date">2021</p>
                </div>
              </div>
            </div>
            <div class="w-full sm:w-1/2 md:w-1/4 self-stretch p-2 mb-2 static">
              <div class="absolute w-192">
                <p class="right-0 relative bx-ractangle">6.5</p>
              </div>
              <div class="rounded shadow-md h-full box-card">
                <router-link to="/detail"
                  ><img
                    class="w-full m-0 rounded-t lazy"
                    src="../assets/movies-10.png"
                    alt="This post thumbnail"
                    width="960"
                    height="500"
                /></router-link>
                <div class="px-0 py-5">
                  <div class="font-semibold text-lg mb-2">
                    <router-link class="text-slate-900 hover:text-slate-700" to="/detail"
                      >Outside the Wire</router-link
                    >
                  </div>
                  <p class="text-slate-700 mb-1" title="Published date">2021</p>
                </div>
              </div>
            </div>
            <!-- next -->
            <div class="w-full sm:w-1/2 md:w-1/4 self-stretch p-2 mb-2 static">
              <div class="absolute w-192">
                <p class="right-0 relative bx-ractangle">5.0</p>
              </div>
              <div class="rounded shadow-md h-full box-card">
                <router-link to="/detail"
                  ><img
                    class="w-full m-0 rounded-t lazy"
                    src="../assets/movies-5.png"
                    alt="This post thumbnail"
                    width="960"
                    height="500"
                /></router-link>
                <div class="px-0 py-5">
                  <div class="font-semibold text-lg mb-2">
                    <router-link class="text-slate-900 hover:text-slate-700" to="/detail"
                      >Breach</router-link
                    >
                  </div>
                  <p class="text-slate-700 mb-1" title="Published date">2021</p>
                </div>
              </div>
            </div>
            <div class="w-full sm:w-1/2 md:w-1/4 self-stretch p-2 mb-2 static">
              <div class="absolute w-192">
                <p class="right-0 relative bx-ractangle">4.0</p>
              </div>
              <div class="rounded shadow-md h-full box-card">
                <router-link to="/detail"
                  ><img
                    class="w-full m-0 rounded-t lazy"
                    src="../assets/movies-6.png"
                    alt="This post thumbnail"
                    width="960"
                    height="500"
                /></router-link>
                <div class="px-0 py-5">
                  <div class="font-semibold text-lg mb-2">
                    <router-link class="text-slate-900 hover:text-slate-700" to="/detail"
                      >Soul</router-link
                    >
                  </div>
                  <p class="text-slate-700 mb-1" title="Published date">2021</p>
                </div>
              </div>
            </div>
            <div class="w-full sm:w-1/2 md:w-1/4 self-stretch p-2 mb-2 static">
              <div class="absolute w-192">
                <p class="right-0 relative bx-ractangle">8.3</p>
              </div>
              <div class="rounded shadow-md h-full box-card">
                <router-link to="/detail"
                  ><img
                    class="w-full m-0 rounded-t lazy"
                    src="../assets/movies-7.png"
                    alt="This post thumbnail"
                    width="960"
                    height="500"
                /></router-link>
                <div class="px-0 py-5">
                  <div class="font-semibold text-lg mb-2">
                    <router-link class="text-slate-900 hover:text-slate-700" to="/detail"
                      >Fast & Furious Present..</router-link
                    >
                  </div>
                  <p class="text-slate-700 mb-1" title="Published date">2019</p>
                </div>
              </div>
            </div>
            <div class="w-full sm:w-1/2 md:w-1/4 self-stretch p-2 mb-2 static">
              <div class="absolute w-192">
                <p class="right-0 relative bx-ractangle">6.9</p>
              </div>
              <div class="rounded shadow-md h-full box-card">
                <router-link to="/detail"
                  ><img
                    class="w-full m-0 rounded-t lazy"
                    src="../assets/movies-8.png"
                    alt="This post thumbnail"
                    width="960"
                    height="500"
                /></router-link>
                <div class="px-0 py-5">
                  <div class="font-semibold text-lg mb-2">
                    <router-link class="text-slate-900 hover:text-slate-700" to="/detail"
                      >The Croods: A New Age</router-link
                    >
                  </div>
                  <p class="text-slate-700 mb-1" title="Published date">2020</p>
                </div>
              </div>
            </div>
            <div class="container py-10 px-10 mx-0 min-w-full flex flex-col items-center">
              <button
                class="px-6 py-2 rounded bg-red hover:bg-rose-500 text-rose-100 btn-radius text-base"
              >
                Load More
              </button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
<script>
import Discover from "@/components/home/Discover.vue";
export default {
  components: {
    Discover,
  },
  data() {
    return {
      isOptionsExpanded: false,
      selectedOption: "Popularity",
      options: ["Action", "Adventure", "Animation", "Comedy"],
    };
  },
  methods: {
    setOption(option) {
      this.selectedOption = option;
      this.isOptionsExpanded = false;
    },
  },
};
</script>
