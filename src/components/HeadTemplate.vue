<template>
  <header
    id="header"
    class="w-full px-6 py-5 z-50 fixed top-0 transition-all transform ease-in-out duration-500 shadow-md"
  >
    <div class="max-w-6xl mx-auto flex items-center flex-wrap justify-between">
      <div class="sm:mr-8">
        <router-link class="flex items-center" to="/"
          ><span class="text-xl text-teal-700 font-semibold self-center"
            ><img
              src="./../assets/icon-movie-head.png"
              class="h-6 mr-3 sm:h-9"
              alt="Flowbite Logo" /></span
        ></router-link>
      </div>
      <form
        id="search"
        action="/search"
        class="order-last sm:order-none flex-grow items-center justify-start sm:block mt-6 sm:mt-0"
        :class="{ hidden: !openNav }"
      >
        <label class="relative block">
          <span class="absolute inset-y-0 left-0 flex items-center pl-3">
            <img src="./../assets/icon_finder_movie.png" class="movie-icon-input" />
          </span>
          <input
            type="text"
            id="header-searchbox"
            name="q"
            placeholder="Find Movie"
            class="w-full bg-slate-200 border border-transparent focus:bg-white focus:border-slate-300 focus:outline-none h-8 p-4 placeholder-slate-500 rounded text-slate-700 text-sm"
          />
          <span class="absolute inset-y-0 right-0 flex items-center pr-3">
            <svg
              class="h-5 w-5 fill-white"
              xmlns="http://www.w3.org/2000/svg"
              x="0px"
              y="0px"
              width="30"
              height="30"
              viewBox="0 0 30 30"
            >
              <path
                d="M 13 3 C 7.4889971 3 3 7.4889971 3 13 C 3 18.511003 7.4889971 23 13 23 C 15.396508 23 17.597385 22.148986 19.322266 20.736328 L 25.292969 26.707031 A 1.0001 1.0001 0 1 0 26.707031 25.292969 L 20.736328 19.322266 C 22.148986 17.597385 23 15.396508 23 13 C 23 7.4889971 18.511003 3 13 3 z M 13 5 C 17.430123 5 21 8.5698774 21 13 C 21 17.430123 17.430123 21 13 21 C 8.5698774 21 5 17.430123 5 13 C 5 8.5698774 8.5698774 5 13 5 z"
              ></path>
            </svg>
          </span>
        </label>
      </form>
      <div
        id="menu-toggle"
        class="flex items-center md:hidden text-slate-700 hover:text-teal-600 cursor-pointer sm:ml-6"
      >
        <svg
          xmlns="http://www.w3.org/2000/svg"
          width="24"
          height="24"
          viewBox="0 0 24 24"
          fill="none"
          stroke="currentColor"
          stroke-width="2"
          stroke-linecap="round"
          stroke-linejoin="round"
          class="feather feather-menu"
          v-on:click="openNavbar"
        >
          <line x1="3" y1="12" x2="21" y2="12"></line>
          <line x1="3" y1="6" x2="21" y2="6"></line>
          <line x1="3" y1="18" x2="21" y2="18"></line>
        </svg>
      </div>

      <nav
        id="menu"
        class="order-last md:order-none items-center flex-grow w-full md:w-auto md:flex mt-2 md:mt-0 pl-10"
        :class="{ hidden: !openNav }"
      >
        <router-link
          to="/about"
          class="block mt-4 md:inline-block md:mt-0 font-medium text-slate-700 hover:text-teal-600 text-base mr-4"
          ><img src="../assets/categories-icon-nav.svg" class="icon-nav"
        /></router-link>
        <router-link
          to="/detail"
          class="block mt-4 md:inline-block md:mt-0 font-medium text-slate-700 hover:text-teal-600 text-base mr-4"
          >Categories</router-link
        >
        <router-link
          to="/bckp"
          class="block mt-4 md:inline-block md:mt-0 font-medium text-slate-700 hover:text-teal-600 text-base mr-4"
          >Moview</router-link
        >
        <a
          href="#"
          target="_blank"
          rel="noopener"
          class="block mt-4 md:inline-block md:mt-0 font-medium text-slate-700 hover:text-teal-600 text-base mr-4"
          >Services</a
        >
        <a
          href="#"
          target="_blank"
          rel="noopener"
          class="block mt-4 md:inline-block md:mt-0 font-medium text-slate-700 hover:text-teal-600 text-base mr-4"
          >Pricing</a
        >
      </nav>
    </div>
  </header>
</template>
<script>
export default {
  data() {
    return {
      openNav: false,
    };
  },
  methods: {
    openNavbar() {
      this.openNav = !this.openNav;
    },
  },
};
</script>
