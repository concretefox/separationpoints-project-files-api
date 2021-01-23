<!-- 02/01/2020
https://www.youtube.com/watch?v=pnkuI8KXW_8&ab_channel=CleverProgrammer

  THIS IS NOW THE MAIN PAGE WORK ON THIS PAGE AND THEN COPY IT OVER TO THE OTHER PAGES AS A TEMPLATE
-->

<template>
  <!-- Top side bar -->
  <div class="flex flex-col h-screen text-sm text-gray-400">
    <div class="flex-1 flex overflow-y-hidden">
      <div
        class="sidebar bg-gray-900-spotify w-48 flex-none flex flex-col justify-between font-semibold"
      >
        <ul class="py-6">
          <li class="border-l-4 border-green-600">
            <a href="/spotify.vue" class="flex items-center mx-4 mt-4 group">
              <svg
                class="fill-current text-white group-hover:text-white h-6 w-6"
                viewBox="0 0 24 24"
                width="24"
                height="24"
              >
                <path
                  d="M13 20v-5h-2v5a2 2 0 01-2 2H6a2 2 0 01-2-2v-7.59l-.3.3a1 1 0 11-1.4-1.42l9-9a1 1 0 011.4 0l9 9a1 1 0 01-1.4 1.42l-.3-.3V20a2 2 0 01-2 2h-3a2 2 0 01-2-2zm5 0v-9.59l-6-6-6 6V20h3v-5c0-1.1.9-2 2-2h2a2 2 0 012 2v5h3z"
                />
              </svg>
              <nuxt-link class="truncate" to="/spotify">Home</nuxt-link>
            </a>
          </li>
          <li class="border-l-4 border-transparent">
            <a href="/about" class="flex items-center mx-4 mt-4 group">
              <svg
                class="fill-current text-white group-hover:text-white h-6 w-6"
                viewBox="0 0 24 24"
                width="24"
                height="24"
              >
                <path
                  d="M13 20v-5h-2v5a2 2 0 01-2 2H6a2 2 0 01-2-2v-7.59l-.3.3a1 1 0 11-1.4-1.42l9-9a1 1 0 011.4 0l9 9a1 1 0 01-1.4 1.42l-.3-.3V20a2 2 0 01-2 2h-3a2 2 0 01-2-2zm5 0v-9.59l-6-6-6 6V20h3v-5c0-1.1.9-2 2-2h2a2 2 0 012 2v5h3z"
                />
              </svg>
              <nuxt-link class="truncate" to="/about">About</nuxt-link>
            </a>
          </li>

          <li class="border-l-4 border-transparent">
            <a href="/about.vue" class="flex items-center mx-4 mt-4 group">
              <svg
                class="fill-current text-white group-hover:text-white h-6 w-6"
                viewBox="0 0 24 24"
                width="24"
                height="24"
              >
                <path
                  d="M13 20v-5h-2v5a2 2 0 01-2 2H6a2 2 0 01-2-2v-7.59l-.3.3a1 1 0 11-1.4-1.42l9-9a1 1 0 011.4 0l9 9a1 1 0 01-1.4 1.42l-.3-.3V20a2 2 0 01-2 2h-3a2 2 0 01-2-2zm5 0v-9.59l-6-6-6 6V20h3v-5c0-1.1.9-2 2-2h2a2 2 0 012 2v5h3z"
                />
              </svg>
              <a
                class=""
                href="https://www.twitch.tv/separationpoints"
                target="blank"
                >Live Stream</a
              >
            </a>
          </li>
        </ul>

        <!-- Side bar -->

        <div class="sidebar-spotify overflow-y-auto px-5 mt-2">
          <h3
            class="uppercase tracking-widest text-gray-500 font-normal text-xs"
          >
            What's On?
          </h3>
          <ul class="leading-extra-loose">
            <li class="hover:text-white">
              <nuxt-link class="truncate" to="/spotify"
                >Monthly Podcast</nuxt-link
              >
            </li>

            <li class="truncat hover:text-white">
              <a
                href="https://www.mixcloud.com/separationpoints/music-from-rio-side-1/"
                target="blank"
                >Music from Rio: Side 1</a
              >
            </li>

            <nuxt-link class="truncate" to="#" hover:text-white
              >Jazz Club(Coming Soon)
            </nuxt-link>
          </ul>

          <!-- Playlists -->
          <h3
            class="uppercase tracking-widest text-gray-500 font-normal text-xs mt-6"
          >
            Interviews
          </h3>
          <ul class="leading-extra-loose mb-6">
            <li class="truncate">
              <a href="#" class="hover:text-white">Coming soon</a>
            </li>
            <li class="truncate">
              <a href="#" class="hover:text-white">Coming soon</a>
            </li>
          </ul>
        </div>
        <div
          class="border-t border-gray-800 h-16 px-4 py-2 flex items-center group"
        >
          <svg
            class="fill-current text-gray-600 w-8 h-8 group-hover:text-white"
            viewBox="0 0 24 24"
            width="24"
            height="24"
          >
            <path
              class="heroicon-ui"
              d="M12 22a10 10 0 110-20 10 10 0 010 20zm0-2a8 8 0 100-16 8 8 0 000 16zm1-9h2a1 1 0 010 2h-2v2a1 1 0 01-2 0v-2H9a1 1 0 010-2h2V9a1 1 0 012 0v2z"
            />
          </svg>
          <a
            href="#"
            class="font-normal text-gray-500 ml-2 group-hover:text-white"
            >New Playlist</a
          >
        </div>
      </div>

      <div class="bg-gray-800-spotify flex-1 flex flex-col">
        <div class="top-bar flex items-center justify-between px-4 py-2">
          <div class="flex items-center">
            <button>
              <svg
                class="fill-current text-gray-400 hover:text-white h-10 w-10"
                viewBox="0 0 24 24"
                width="24"
                height="24"
              >
                <path
                  d="M14.7 15.3a1 1 0 01-1.4 1.4l-4-4a1 1 0 010-1.4l4-4a1 1 0 011.4 1.4L11.42 12l3.3 3.3z"
                />
              </svg>
            </button>
            <button class="ml-1">
              <svg
                class="fill-current text-gray-400 hover:text-white h-10 w-10"
                viewBox="0 0 24 24"
                width="24"
                height="24"
              >
                <path
                  class="heroicon-ui"
                  d="M9.3 8.7a1 1 0 011.4-1.4l4 4a1 1 0 010 1.4l-4 4a1 1 0 01-1.4-1.4l3.29-3.3-3.3-3.3z"
                />
              </svg>
            </button>
            <div class="ml-4 relative">
              <input
                type="text"
                placeholder="Search"
                class="bg-white text-gray-800 placeholder-gray-800 rounded-full px-3 pl-8 py-1"
              />
              <div class="absolute top-0">
                <svg
                  class="fill-current text-gray-800 h-6 w-6 pt-1 pl-2"
                  viewBox="0 0 24 24"
                  width="24"
                  height="24"
                >
                  <path
                    class="heroicon-ui"
                    d="M16.32 14.9l5.39 5.4a1 1 0 01-1.42 1.4l-5.38-5.38a8 8 0 111.41-1.41zM10 16a6 6 0 100-12 6 6 0 000 12z"
                  />
                </svg>
              </div>
            </div>
          </div>
          <div class="flex items-center">
            <button>
              <svg
                class="fill-current text-gray-400 hover:text-white w-6 h-6"
                viewBox="0 0 496 512"
              >
                <path
                  d="M248 104c-53 0-96 43-96 96s43 96 96 96 96-43 96-96-43-96-96-96zm0 144c-26.5 0-48-21.5-48-48s21.5-48 48-48 48 21.5 48 48-21.5 48-48 48zm0-240C111 8 0 119 0 256s111 248 248 248 248-111 248-248S385 8 248 8zm0 448c-49.7 0-95.1-18.3-130.1-48.4 14.9-23 40.4-38.6 69.6-39.5 20.8 6.4 40.6 9.6 60.5 9.6s39.7-3.1 60.5-9.6c29.2 1 54.7 16.5 69.6 39.5-35 30.1-80.4 48.4-130.1 48.4zm162.7-84.1c-24.4-31.4-62.1-51.9-105.1-51.9-10.2 0-26 9.6-57.6 9.6-31.5 0-47.4-9.6-57.6-9.6-42.9 0-80.6 20.5-105.1 51.9C61.9 339.2 48 299.2 48 256c0-110.3 89.7-200 200-200s200 89.7 200 200c0 43.2-13.9 83.2-37.3 115.9z"
                />
              </svg>
            </button>
            <a href="#" class="ml-2 hover:underline hover:text-white"
              >Separation Points</a
            >
            <button class="ml-4">
              <svg
                class="fill-current text-gray-400 hover:text-white w-6 h-6"
                viewBox="0 0 24 24"
                width="24"
                height="24"
              >
                <path
                  class="heroicon-ui"
                  d="M15.3 9.3a1 1 0 011.4 1.4l-4 4a1 1 0 01-1.4 0l-4-4a1 1 0 011.4-1.4l3.3 3.29 3.3-3.3z"
                />
              </svg>
            </button>
          </div>
        </div>
        <div class="content-spotify overflow-y-auto">
          <div class="container mx-auto">
            <h2 class="mt-24 text-5xl font-semibold">Welcome Back</h2>

            <!-- Featured shows areas -->
            <div class="mt-12">
              <h3 class="font-semibold text-xl border-b border-gray-900 pb-2">
                <nuxt-link class="truncate" to="/podcasts"
                  >The Latest podcasts</nuxt-link
                >
              </h3>
              <div class="flex items-center mt-4 -mx-4">
                <!-- Podcast item -->
                <div class="w-1/5 px-4">
                  <div>
                    <a href="#"
                      ><img
                        alt="#038 - Spaven x Sandunes EP, Brazilian Funk, Bossa Nova & classic Brazilian vibes"
                        src="~/assets/img/podcast/thumbnails/038-podcast.jpg"
                        srcset=""
                        height="300"
                        width="300"
                        style="display: block; opacity: 1"
                    /></a>
                  </div>
                  <div>
                    <!-- Title -->
                    <a
                      href="#"
                      class="font-semibold block hover:text-white mt-2"
                      @click="podcast038"
                      >#038 - Spaven x Sandunes EP</a
                    >
                    <!-- Description -->
                    <div class="text-gray-500 mt-2"></div>
                    <div
                      class="uppercase tracking-widest text-xs text-gray-500 mt-2"
                    >
                      Broadcasted on 01/11/2020
                    </div>
                  </div>
                </div>
                <!-- Podcast item END -->

                <!-- Podcast item -->
                <div class="w-1/5 px-4">
                  <div>
                    <a href="#"
                      ><img
                        alt="#037 - Bairro Alto Brazilika & Friends"
                        src="~/assets/img/podcast/thumbnails/generic-podcast.png"
                        srcset=""
                        height="300"
                        width="300"
                        style="display: block; opacity: 1"
                    /></a>
                  </div>
                  <div>
                    <!-- Title -->
                    <a
                      href="#"
                      class="font-semibold block hover:text-white mt-2"
                      v-on:click="podcast037"
                      >#037 - Bairro Alto Brazilika
                    </a>
                    <!-- Description -->
                    <div class="text-gray-500 mt-2"></div>
                    <div
                      class="uppercase tracking-widest text-xs text-gray-500 mt-2"
                    >
                      Broadcasted on 01/11/2020
                    </div>
                  </div>
                </div>
                <!-- Podcast item END -->

                <div class="w-1/5 px-4">
                  <div>
                    <a href="#"
                      ><img
                        src="~/assets/img/podcast/thumbnails/generic-podcast.png"
                        alt="#036 - 10 Years of Gondwana Records & Matthew Halsall"
                    /></a>
                  </div>
                  <div>
                    <a
                      href="#"
                      class="font-semibold block hover:text-white mt-2"
                      v-on:click="podcast036"
                      >#036 - 10 Years of Gondwana Records part 2
                    </a>
                    <div class="text-gray-500 mt-2"></div>
                    <div
                      class="uppercase tracking-widest text-xs text-gray-500 mt-2"
                    >
                      Broadcasted on 01/10/2020
                    </div>
                  </div>
                </div>

                <div class="w-1/5 px-4">
                  <div>
                    <a href="#"
                      ><img
                        src="~/assets/img/podcast/thumbnails/generic-podcast.png"
                        alt="album cover"
                    /></a>
                  </div>
                  <div>
                    <a
                      href="#"
                      alt="El Búho, Celt Islam, Freeeze, Elkin & Nelson, Acid Arab,
                      Alborosie and more!"
                      class="font-semibold block hover:text-white mt-2"
                      v-on:click="podcast035"
                      >#035- El Búho, Celt Islam, Freeeze, Elkin & Nelson, Acid
                      Arab, Alborosie and more!</a
                    >
                    <div class="text-gray-500 mt-2"></div>
                    <div
                      class="uppercase tracking-widest text-xs text-gray-500 mt-2"
                    >
                      Broadcasted on 01/09/2020
                    </div>
                  </div>
                </div>

                <div class="w-1/5 px-4">
                  <div>
                    <a href="#"
                      ><img
                        src="~/assets/img/podcast/thumbnails/generic-podcast.png"
                        alt="album cover"
                    /></a>
                  </div>
                  <div>
                    <a
                      href="#"
                      class="font-semibold block hover:text-white mt-2"
                      v-on:click="podcast034"
                      >#034 - FKJ, Nubya Garcia,Tony Allen, MJ Cole, Four Tet,
                      HAAi, Minor Science and more!</a
                    >
                    <div class="text-gray-500 mt-2"></div>
                    <div
                      class="uppercase tracking-widest text-xs text-gray-500 mt-2"
                    >
                      Broadcasted on 01/08/2020
                    </div>
                  </div>
                </div>
              </div>
            </div>

            <!-- Next Row -->
            <div class="mt-12">
              <h3 class="font-semibold text-xl border-b border-gray-900 pb-2">
                Live from the Loft
              </h3>
              <div class="flex items-center mt-4 -mx-4">
                <div class="w-1/5 px-4">
                  <div>
                    <a href="#"
                      ><img
                        src="~assets/img/live from the loft/thumbnails/live-from-the-loft-1.png"
                        alt="#033 - Steam Down, Aditya Prakash, St. Germain, El Búho,
                      Clozee, Anna Meredith, Jimi Hendrix"
                    /></a>
                  </div>
                  <div>
                    <a
                      href="#"
                      class="font-semibold block hover:<text-white mt-2"
                      >Live from The Loft - 06/11/2020
                    </a>
                    <div class="text-gray-500 mt-2"></div>
                    <div
                      class="uppercase tracking-widest text-xs text-gray-500 mt-2"
                    >
                      BROADCAST ON 6/11/2020
                    </div>
                  </div>
                </div>

                <div class="w-1/5 px-4">
                  <div>
                    <a href="#"
                      ><img
                        src="~assets/img/live from the loft/thumbnails/live-from-the-loft-1.png"
                        alt="album cover"
                    /></a>
                  </div>
                  <div>
                    <a
                      href="#"
                      class="font-semibold block hover:text-white mt-2"
                      >A Latin Special - 20-11-2020</a
                    >

                    <div class="text-gray-500 mt-2">
                      Broadcasted on 20-11-2020
                    </div>
                    <div
                      class="uppercase tracking-widest text-xs text-gray-500 mt-2"
                    >
                      6679 Followers
                    </div>
                  </div>
                </div>
              </div>
            </div>

            <!-- Next Row -->
            <div class="mt-12 mb-12">
              <h3 class="font-semibold text-xl border-b border-gray-900 pb-2">
                <nuxt-link class="truncate" to="#"
                  >Jazz Club (Coming Soon)</nuxt-link
                >
              </h3>
            </div>

            <!-- Next Row -->
            <div class="mt-12 mb-12">
              <h3 class="font-semibold text-xl border-b border-gray-900 pb-2">
                <nuxt-link class="truncate" to="#"
                  >Reggea Cuts (Coming Soon)</nuxt-link
                >
              </h3>
            </div>
          </div>
        </div>
      </div>
    </div>

    <!-- Player Bar -->
    <iframe
      width="100%"
      height="120"
      src="https://www.mixcloud.com/widget/iframe/?hide_cover=1&feed=%2Fseparationpoints%2F038-spaven-x-sandunes-ep-brazilian-funk-and-some-more-bossa-nova-classic-brazilian-vibes%2F"
      frameborder="0"
    ></iframe>
  </div>
  <!--
  <div>
    
    <iframe
      id="mixcloud"
      :src="link"
      @load="mountApi"
      width="100%"
      height="120"
      frameborder="0"
      allow="autoplay"
    >
    </iframe>
  </div>
  -->
</template>


<script>
// window.axios = require("axios");
// v-for="post in posts" v-text="post.title"//

import axios from "axios";

export default {
  methods: {
    podcast038() {
      // console.log("038 Podcast has been clicked");
      // alert("038 Podcast has been clicked");

      // Here we use VueJS refs instead of directly trageting the DOM in tradional JS ways//
      // We assign refs to elements and then target them and to replace the src HTML to hopefully load the content into the player//

      // this.$refs.MixCloudPlayer.src.innerHTML =
      // "https://www.mixcloud.com/separationpoints/038-spaven-x-sandunes-ep-brazilian-funk-and-some-more-bossa-nova-classic-brazilian-vibes/";

      console.log(this.$refs.MixCloudPlayer);
    },

    podcast038API() {},

    podcast034: function (event) {
      // `this` inside methods points to the Vue instance
      alert("You clicked on 034 " + this.name + "!");

      document.getElementById("mixcloud-player").src.innerHTML = "";

      // `event` is the native DOM event
      if (event) {
        alert(event.target.tagName);
      }
    },
  },

  // When the app is mounted is will called Axios and then post it in the console //

  mounted() {
    axios
      .get("https://jsonplaceholder.typicode.com/posts")
      .then((response) => console.log(response));

    //.then((response) => (this.posts = response.data));
    //console.log(this.posts);
  },

  data() {
    posts: null;
    return {};
  },
};
</script>


<style>
.sidebar-spotify::-webkit-scrollbar {
  width: 8px;
  background-color: #121212;
}

.sidebar-spotify::-webkit-scrollbar-thumb {
  border-radius: 8px;
  background-color: #535353;
}

.content-spotify::-webkit-scrollbar {
  width: 8px;
  background-color: #181818;
}

.content-spotify::-webkit-scrollbar-thumb {
  border-radius: 8px;
  background-color: #535353;
}
</style>
