<template>
  <div class="flex flex-col h-screen text-sm text-gray-400">
    <div class="flex-1 flex overflow-y-hidden">
      <div
        class="sidebar bg-gray-900-spotify w-48 flex-none flex flex-col justify-between font-semibold"
      >
        <ul class="py-6">
          <li class="border-l-4 border-green-600">
            <a href="#" class="flex items-center mx-4 mt-4 group">
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
              <!-- <span class="ml-2 text-white group-hover:text-white">Home</span> -->
              <nuxt-link
                class="truncate ml-2"
                to="../pages/spotify"
                hover:text-white
                >Home</nuxt-link
              >
            </a>
          </li>
          <li class="border-l-4 border-transparent">
            <a
              href="#"
              class="flex items-center hover:text-white mx-4 mt-4 group"
            >
              <svg
                class="fill-current text-gray-400 h-6 w-6 group-hover:text-white"
                width="24"
                height="24"
              >
                <path fill="none" d="M15 5.414V7h1.586z" />
                <path fill="none" d="M14 9a1 1 0 01-1-1V4H9v12h9V9h-4z" />
                <path
                  d="M20 17V8h-.009a.996.996 0 00-.284-.707l-5-5A.99.99 0 0014 2.01V2H8a1 1 0 00-1 1v14a1 1 0 001 1h11a1 1 0 001-1zM15 5.414L16.586 7H15V5.414zM9 16V4h4v4a1 1 0 001 1h4v7H9z"
                />
                <path d="M3 8v13a1 1 0 001 1h12v-2H5V8H3z" />
              </svg>

              <nuxt-link
                class="truncate ml-2"
                to="../pages/browse"
                hover:text-white
                >Browse</nuxt-link
              >
            </a>
          </li>
          <li class="border-l-4 border-transparent">
            <a
              href="#"
              class="flex items-center hover:text-white mx-4 mt-4 group"
            >
              <svg
                class="fill-current text-gray-400 h-6 w-6 group-hover:text-white"
                viewBox="0 0 24 24"
              >
                <g data-name="Layer 2">
                  <g data-name="radio">
                    <path
                      d="M12 8a3 3 0 00-1 5.83 1 1 0 000 .17v6a1 1 0 002 0v-6a1 1 0 000-.17A3 3 0 0012 8zm0 4a1 1 0 111-1 1 1 0 01-1 1zM3.5 11a6.87 6.87 0 012.64-5.23 1 1 0 10-1.28-1.54A8.84 8.84 0 001.5 11a8.84 8.84 0 003.36 6.77 1 1 0 101.28-1.54A6.87 6.87 0 013.5 11z"
                    />
                    <path
                      d="M16.64 6.24a1 1 0 00-1.28 1.52A4.28 4.28 0 0117 11a4.28 4.28 0 01-1.64 3.24A1 1 0 0016 16a1 1 0 00.64-.24A6.2 6.2 0 0019 11a6.2 6.2 0 00-2.36-4.76zM8.76 6.36a1 1 0 00-1.4-.12A6.2 6.2 0 005 11a6.2 6.2 0 002.36 4.76 1 1 0 001.4-.12 1 1 0 00-.12-1.4A4.28 4.28 0 017 11a4.28 4.28 0 011.64-3.24 1 1 0 00.12-1.4z"
                    />
                    <path
                      d="M19.14 4.23a1 1 0 10-1.28 1.54A6.87 6.87 0 0120.5 11a6.87 6.87 0 01-2.64 5.23 1 1 0 001.28 1.54A8.84 8.84 0 0022.5 11a8.84 8.84 0 00-3.36-6.77z"
                    />
                  </g>
                </g>
              </svg>
              <nuxt-link
                class="truncate ml-2"
                to="../pages/radio"
                hover:text-white
                >Radio</nuxt-link
              >
            </a>
          </li>
        </ul>

        <div class="sidebar-spotify overflow-y-auto px-5 mt-3">
          <h3
            class="uppercase tracking-widest text-gray-500 font-normal text-xs"
          >
            Your Library
          </h3>
          <ul class="leading-extra-loose">
            <!-- Just like router-link you add views or pages in this case to Nuxt JS like so -->

            <nuxt-link class="truncate" to="/podcasts" hover:text-white
              >Monthly Podcast</nuxt-link
            >
            <nuxt-link class="truncate" to="/theloft" hover:text-white
              >Live from The Loft</nuxt-link
            >
            <nuxt-link class="truncate" to="/theloft" hover:text-white
              >Reggae Cuts</nuxt-link
            >
            <nuxt-link class="truncate" to="/jazzclub" hover:text-white
              >Jazz Club</nuxt-link
            >
          </ul>

          <!-- 
            <li class="truncate"><a href="#" class="hover:text-white">Liked Songs</a></li>
            <li class="truncate"><a href="#" class="hover:text-white">Albums</a></li> 
            <li class="truncate"><a href="#" class="hover:text-white">Artists</a></li>
            <li class="truncate"><a href="#" class="hover:text-white">Podcasts</a></li>

-->

          <h3
            class="uppercase tracking-widest text-gray-500 font-normal text-xs mt-6"
          >
            Playlists
          </h3>
          <ul class="leading-extra-loose mb-6">
            <li class="truncate">
              <a href="#" class="hover:text-white">R&amp;B Right Now</a>
            </li>
            <li class="truncate">
              <a href="#" class="hover:text-white">I Love My '90s R&amp;B</a>
            </li>
            <li class="truncate">
              <a href="#" class="hover:text-white">Are &amp; Be</a>
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
              >dredrehimself</a
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

          <!-- Main titles -->
        </div>

        <div class="content-spotify overflow-y-auto">
          <div class="container mx-auto">
            <h2 class="mt-24 text-5xl font-semibold text-white">
              Let's have a browse
            </h2>

            <div class="mt-12">
              <h3 class="font-semibold text-xl border-b border-gray-900 pb-2">
                Recently Played
              </h3>
              <div class="flex items-center mt-4 -mx-4">
                <div class="w-1/5 px-4">
                  <div>
                    CH
                    <a href="#"
                      ><img src="/albumcover02.jpg" alt="album cover"
                    /></a>
                  </div>
                  <div>
                    <a
                      href="#"
                      class="font-semibold block hover:text-white mt-2"
                      >Acoustic Pop Covers 2019</a
                    >
                    <div class="text-gray-500 mt-2">
                      Amazing Acoustic Covers updated every week.
                    </div>
                    <div
                      class="uppercase tracking-widest text-xs text-gray-500 mt-2"
                    >
                      6679 Followers
                    </div>
                  </div>
                </div>

                <div class="w-1/5 px-4">
                  <div>
                    <a href="#"
                      ><img src="/albumcover03.jpg" alt="album cover"
                    /></a>
                  </div>
                  <div>
                    <a
                      href="#"
                      class="font-semibold block hover:text-white mt-2"
                      >Podcast #37</a
                    >
                    <div class="text-gray-500 mt-2">
                      Amazing Acoustic Covers updated every week.
                    </div>
                    <div
                      class="uppercase tracking-widest text-xs text-gray-500 mt-2"
                    >
                      6679 Followers
                    </div>
                  </div>
                </div>

                <div class="w-1/5 px-4">
                  <div>
                    <a href="#"
                      ><img src="/albumcover04.jpg" alt="album cover"
                    /></a>
                  </div>
                  <div>
                    <a
                      href="#"
                      class="font-semibold block hover:text-white mt-2"
                      >Podcast #36</a
                    >
                    <div class="text-gray-500 mt-2">
                      Amazing Acoustic Covers updated every week.
                    </div>
                    <div
                      class="uppercase tracking-widest text-xs text-gray-500 mt-2"
                    >
                      6679 Followers
                    </div>
                  </div>
                </div>

                <div class="w-1/5 px-4">
                  <div>
                    <a href="#"
                      ><img src="/albumcover05.jpg" alt="album cover"
                    /></a>
                  </div>
                  <div>
                    <a
                      href="#"
                      class="font-semibold block hover:text-white mt-2"
                      >Podcast #36</a
                    >
                    <div class="text-gray-500 mt-2">
                      Amazing Acoustic Covers updated every week.
                    </div>
                    <div
                      class="uppercase tracking-widest text-xs text-gray-500 mt-2"
                    >
                      6679 Followers
                    </div>
                  </div>
                </div>

                <div class="w-1/5 px-4">
                  <div>
                    <a href="#"
                      ><img src="/albumcover06.jpg" alt="album cover"
                    /></a>
                  </div>
                  <div>
                    <a
                      href="#"
                      class="font-semibold block hover:text-white mt-2"
                      >Podcast #35</a
                    >
                    <div class="text-gray-500 mt-2">
                      Amazing Acoustic Covers updated every week.
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

            <div class="mt-12">
              <h3 class="font-semibold text-xl border-b border-gray-900 pb-2">
                Your Heavy Rotation
              </h3>
              <div class="flex items-center mt-4 -mx-4">
                <div class="w-1/5 px-4">
                  <div>
                    <a href="#"
                      ><img src="/albumcover06.jpg" alt="album cover"
                    /></a>
                  </div>
                  <div>
                    <a
                      href="#"
                      class="font-semibold block hover:text-white mt-2"
                      >Podcast #35</a
                    >
                    <div class="text-gray-500 mt-2">
                      Amazing Acoustic Covers updated every week.
                    </div>
                    <div
                      class="uppercase tracking-widest text-xs text-gray-500 mt-2"
                    >
                      6679 Followers
                    </div>
                  </div>
                </div>

                <div class="w-1/5 px-4">
                  <div>
                    <a href="#"
                      ><img src="/albumcover05.jpg" alt="album cover"
                    /></a>
                  </div>
                  <div>
                    <a
                      href="#"
                      class="font-semibold block hover:text-white mt-2"
                      >Podcast #34</a
                    >
                    <div class="text-gray-500 mt-2">
                      Amazing Acoustic Covers updated every week.
                    </div>
                    <div
                      class="uppercase tracking-widest text-xs text-gray-500 mt-2"
                    >
                      6679 Followers
                    </div>
                  </div>
                </div>

                <div class="w-1/5 px-4">
                  <div>
                    <a href="#"
                      ><img src="/albumcover04.jpg" alt="album cover"
                    /></a>
                  </div>
                  <div>
                    <a
                      href="#"
                      class="font-semibold block hover:text-white mt-2"
                      >Podcast #33</a
                    >
                    <div class="text-gray-500 mt-2">
                      Amazing Acoustic Covers updated every week.
                    </div>
                    <div
                      class="uppercase tracking-widest text-xs text-gray-500 mt-2"
                    >
                      6679 Followers
                    </div>
                  </div>
                </div>

                <div class="w-1/5 px-4">
                  <div>
                    <a href="#"
                      ><img src="/albumcover03.jpg" alt="album cover"
                    /></a>
                  </div>
                  <div>
                    <a
                      href="#"
                      class="font-semibold block hover:text-white mt-2"
                      >Podcast #32</a
                    >
                    <div class="text-gray-500 mt-2">
                      Amazing Acoustic Covers updated every week.
                    </div>
                    <div
                      class="uppercase tracking-widest text-xs text-gray-500 mt-2"
                    >
                      6679 Followers
                    </div>
                  </div>
                </div>

                <div class="w-1/5 px-4">
                  <div>
                    <a href="#"
                      ><img src="/albumcover02.jpg" alt="album cover"
                    /></a>
                  </div>
                  <div>
                    <a
                      href="#"
                      class="font-semibold block hover:text-white mt-2"
                      >Podcast #31</a
                    >
                    <div class="text-gray-500 mt-2">
                      Amazing Acoustic Covers updated every week.
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

            <div class="mt-12 mb-12">
              <h3 class="font-semibold text-xl border-b border-gray-900 pb-2">
                Chill
              </h3>
              <div class="flex items-center mt-4 -mx-4">
                <div class="w-1/5 px-4">
                  <div>
                    <a href="#"
                      ><img src="/albumcover02.jpg" alt="album cover"
                    /></a>
                  </div>
                  <div>
                    <a
                      href="#"
                      class="font-semibold block hover:text-white mt-2"
                      >Podcast #30</a
                    >
                    <div class="text-gray-500 mt-2">
                      Amazing Acoustic Covers updated every week.
                    </div>
                    <div
                      class="uppercase tracking-widest text-xs text-gray-500 mt-2"
                    >
                      6679 Followers
                    </div>
                  </div>
                </div>

                <div class="w-1/5 px-4">
                  <div>
                    <a href="#"
                      ><img src="/albumcover03.jpg" alt="album cover"
                    /></a>
                  </div>
                  <div>
                    <a
                      href="#"
                      class="font-semibold block hover:text-white mt-2"
                      >Podcast #29</a
                    >
                    <div class="text-gray-500 mt-2">
                      Amazing Acoustic Covers updated every week.
                    </div>
                    <div
                      class="uppercase tracking-widest text-xs text-gray-500 mt-2"
                    >
                      6679 Followers
                    </div>
                  </div>
                </div>

                <div class="w-1/5 px-4">
                  <div>
                    <a href="#"
                      ><img src="/albumcover04.jpg" alt="album cover"
                    /></a>
                  </div>
                  <div>
                    <a
                      href="#"
                      class="font-semibold block hover:text-white mt-2"
                      >Podcast #28</a
                    >
                    <div class="text-gray-500 mt-2">
                      Amazing Acoustic Covers updated every week.
                    </div>
                    <div
                      class="uppercase tracking-widest text-xs text-gray-500 mt-2"
                    >
                      6679 Followers
                    </div>
                  </div>
                </div>

                <div class="w-1/5 px-4">
                  <div>
                    <a href="#"
                      ><img src="/albumcover05.jpg" alt="album cover"
                    /></a>
                  </div>
                  <div>
                    <a
                      href="#"
                      class="font-semibold block hover:text-white mt-2"
                      >Podcast #27</a
                    >
                    <div class="text-gray-500 mt-2">
                      Amazing Acoustic Covers updated every week.
                    </div>
                    <div
                      class="uppercase tracking-widest text-xs text-gray-500 mt-2"
                    >
                      6679 Followers
                    </div>
                  </div>
                </div>

                <div class="w-1/5 px-4">
                  <div>
                    <a href="#"
                      ><img src="/albumcover06.jpg" alt="album cover"
                    /></a>
                  </div>
                  <div>
                    <a
                      href="#"
                      class="font-semibold block hover:text-white mt-2"
                      >Acoustic Pop Covers 2019</a
                    >
                    <div class="text-gray-500 mt-2">
                      Amazing Acoustic Covers updated every week.
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
          </div>
        </div>
      </div>
    </div>

    <!-- Player Bar 
      JSON Data - https://www.mixcloud.com/oembed/?url=https%3A%2F%2Fwww.mixcloud.com%2Fseparationpoints%2Fseparationpoints%2F038-spaven-x-sandunes-ep-brazilian-funk-and-some-more-bossa-nova-classic-brazilian-vibes%2F&format=json


      Fuctional player
      <iframe width="100%" height="120" src="https://www.mixcloud.com/widget/iframe/?hide_cover=1&feed=%2Fseparationpoints%2F038-spaven-x-sandunes-ep-brazilian-funk-and-some-more-bossa-nova-classic-brazilian-vibes%2F" frameborder="0" ></iframe>
  
      -->
    <div class="w-100">
      <MixcloudPlayer />
    </div>
  </div>
</template>

<script>
export default {
  // For loading external scripts onto page //
  head() {
    return {
      script: [
        {
          rel: "javascript",
          src: "//widget.mixcloud.com/media/js/widgetApi.js",
        },
      ],

      link: [
        {
          rel: "stylesheet",
          href: "https://fonts.googleapis.com/css?family=Roboto&display=swap",
        },
      ],
    };
  },

  // where I can store data for API? //
  data() {
    [
      {
        id: "038",
        title:
          "#038 - Spaven x Sandunes EP, Brazilian Funk, Bossa Nova & classic Brazilian vibes",
        description: "Spaven x Sandunes released on th 11th September 2020.",
      },
    ];
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
