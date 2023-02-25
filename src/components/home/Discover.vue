<template>
  <div class="mx-7 lg:mx-6 mt-32 flex-grow">
    <div class="max-w-6xl mx-auto mx-auto">
      <div class="rectangle"></div>
      <h1 class="text-3xl leading-normal font-bold mt-0 mb-7 label-discover pt-28">
        Discover Movies
        <button class="rounded-full float-right bg-black btn-radius">Release Date</button>
        <button class="rounded-full float-right bg-red btn-radius">Popularity</button>
      </h1>
      <div class="flex flex-wrap -mx-2">
        <div class="w-full sm:w-1/2 md:w-1/5 self-stretch p-2 mb-2 static">
          <div class="absolute w-192">
            <p class="right-0 relative bx-ractangle">7.0</p>
          </div>
          <div class="rounded shadow-md h-full box-card">
            <router-link to="/detail"
              ><img
                class="w-full m-0 rounded-t lazy"
                src="../../assets/movies-1.png"
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
        <div class="w-full sm:w-1/2 md:w-1/5 self-stretch p-2 mb-2 static">
          <div class="absolute w-192">
            <p class="right-0 relative bx-ractangle">64</p>
          </div>
          <div class="rounded shadow-md h-full box-card">
            <router-link to="/detail"
              ><img
                class="w-full m-0 rounded-t lazy"
                src="../../assets/movies-2.png"
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
        <div class="w-full sm:w-1/2 md:w-1/5 self-stretch p-2 mb-2 static">
          <div class="absolute w-192">
            <p class="right-0 relative bx-ractangle">6.4</p>
          </div>
          <div class="rounded shadow-md h-full box-card">
            <router-link to="/detail"
              ><img
                class="w-full m-0 rounded-t lazy"
                src="../../assets/movies-3.png"
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
        <div class="w-full sm:w-1/2 md:w-1/5 self-stretch p-2 mb-2 static">
          <div class="absolute w-192">
            <p class="right-0 relative bx-ractangle">6.5</p>
          </div>
          <div class="rounded shadow-md h-full box-card">
            <router-link to="/detail"
              ><img
                class="w-full m-0 rounded-t lazy"
                src="../../assets/movies-10.png"
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

        <div class="w-full sm:w-1/2 md:w-1/5 self-stretch p-2 mb-2 static">
          <div class="absolute w-192">
            <p class="right-0 relative bx-ractangle">5.0</p>
          </div>
          <div class="rounded shadow-md h-full box-card">
            <router-link to="/detail"
              ><img
                class="w-full m-0 rounded-t lazy"
                src="../../assets/movies-5.png"
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
        <div class="w-full sm:w-1/2 md:w-1/5 self-stretch p-2 mb-2 static">
          <div class="absolute w-192">
            <p class="right-0 relative bx-ractangle">4.0</p>
          </div>
          <div class="rounded shadow-md h-full box-card">
            <router-link to="/detail"
              ><img
                class="w-full m-0 rounded-t lazy"
                src="../../assets/movies-6.png"
                alt="This post thumbnail"
                width="960"
                height="500"
            /></router-link>
            <div class="px-0 py-5">
              <div class="font-semibold text-lg mb-2">
                <a class="text-slate-900 hover:text-slate-700" to="/detail">Soul</a>
              </div>
              <p class="text-slate-700 mb-1" title="Published date">2021</p>
            </div>
          </div>
        </div>
        <div class="w-full sm:w-1/2 md:w-1/5 self-stretch p-2 mb-2 static">
          <div class="absolute w-192">
            <p class="right-0 relative bx-ractangle">8.3</p>
          </div>
          <div class="rounded shadow-md h-full box-card">
            <router-link to="/detail"
              ><img
                class="w-full m-0 rounded-t lazy"
                src="../../assets/movies-7.png"
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
        <div class="w-full sm:w-1/2 md:w-1/5 self-stretch p-2 mb-2 static">
          <div class="absolute w-192">
            <p class="right-0 relative bx-ractangle">6.9</p>
          </div>
          <div class="rounded shadow-md h-full box-card">
            <router-link to="/detail"
              ><img
                class="w-full m-0 rounded-t lazy"
                src="../../assets/movies-8.png"
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
        <div class="w-full sm:w-1/2 md:w-1/5 self-stretch p-2 mb-2 static">
          <div class="absolute w-192">
            <p class="right-0 relative bx-ractangle">7.6</p>
          </div>
          <div class="rounded shadow-md h-full box-card">
            <router-link to="/detail"
              ><img
                class="w-full m-0 rounded-t lazy"
                src="../../assets/movies-9.png"
                alt="This post thumbnail"
                width="960"
                height="500"
            /></router-link>
            <div class="px-0 py-5">
              <div class="font-semibold text-lg mb-2">
                <a class="text-slate-900 hover:text-slate-700" to="/detail">Vanguard</a>
              </div>
              <p class="text-slate-700 mb-1" title="Published date">2020</p>
            </div>
          </div>
        </div>
        <div class="w-full sm:w-1/2 md:w-1/5 self-stretch p-2 mb-2 static">
          <div class="absolute w-192">
            <p class="right-0 relative bx-ractangle">6.3</p>
          </div>
          <div class="rounded shadow-md h-full box-card">
            <router-link to="/detail"
              ><img
                class="w-full m-0 rounded-t lazy"
                src="../../assets/movies-10.png"
                alt="This post thumbnail"
                width="960"
                height="500"
            /></router-link>
            <div class="px-0 py-5">
              <div class="font-semibold text-lg mb-2">
                <a class="text-slate-900 hover:text-slate-700" to="/detail"
                  >Black Water: Abyss</a
                >
              </div>
              <p class="text-slate-700 mb-1" title="Published date">2020</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
