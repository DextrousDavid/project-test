<template>
  <header>
    <!-- navbar starts here -->
    <!-- adjust padding 4 to add or remove padding from logo -->
    <nav
      class="flex flex-wrap justify-between items-center bg-white p-4 pt-8 pb-8"
    >
      <div class="flex flex-shrink-0 text-black mb-2 xl:mr-16">
        <nuxt-link
          to="/"
          class="flex items-center md:ml-8 flex-shrink-0 text-black"
        >
          <img src="~/assets/Cloudenly.svg" alt="CloudenlyLogo" />
          <h1 class="ml-1 font-black logo-text">Cloudenly</h1>
        </nuxt-link>
      </div>

      <div class="block lg:hidden">
        <button
          type="button"
          class="flex items-center px-3 py-2 border rounded text-black focus:outline-none outline-none shadow-md"
          @click="isOpen = !isOpen"
        >
          <svg
            class="fill-current h-4 w-4"
            viewBox="0 0 20 20"
            xmlns="http://www.w3.org/2000/svg"
          >
            <title>Menu</title>
            <path d="M0 3h20v2H0V3zm0 6h20v2H0V9zm0 6h20v2H0v-2z" />
          </svg>
        </button>
      </div>

      <!-- display block - Lists -->
      <div
        :class="isOpen ? 'block' : 'hidden'"
        class="w-full block flex-grow lg:flex lg:items-center lg:w-auto font-normal md:ml-24"
      >
        <div class="text-sm lg:flex-grow" @click="isOpen = !isOpen">
          <!-- Product link -->
          <nuxt-link
            to="/userguide"
            class="text-left block mt-4 lg:inline-block lg:mt-0 text-blue-500 py-1 hover:bg-gray-200 rounded mr-3 lg:mr-5"
          >
            User Guide
          </nuxt-link>
          <nuxt-link
            to="/"
            class="text-left block mt-2 lg:inline-block lg:mt-0 text-black py-1 hover:bg-gray-200 rounded mr-3 lg:mr-5"
          >
            Whitepaper
          </nuxt-link>
          <nuxt-link
            to="/"
            class="text-left block mt-2 lg:inline-block lg:mt-0 text-black px-1 py-1 hover:bg-gray-200 rounded mr-3 lg:mr-5"
          >
            Blogs
          </nuxt-link>

          <nuxt-link
            to="/"
            class="text-left block mt-2 lg:inline-block lg:mt-0 text-black-200 px-1 py-1 hover:bg-gray-200 rounded mr-3 lg:mr-5"
          >
            Community
          </nuxt-link>

          <nuxt-link
            to="/"
            class="text-left block mt-2 lg:inline-block lg:mt-0 text-black-200 px-1 py-1 hover:bg-gray-200 rounded mr-3 lg:mr-5"
          >
            Developer Documentation
          </nuxt-link>

          <nuxt-link
            to="/"
            class="text-left block mt-2 lg:inline-block lg:mt-0 text-black-200 px-1 py-1 hover:bg-gray-200 rounded mr-2"
          >
            Events
          </nuxt-link>
        </div>
      </div>
    </nav>
  </header>
</template>

<script>
export default {
  name: 'Header',
  data() {
    return {
      isOpen: false,
    }
  },
  head() {
    return {
      link: [
        {
          rel: 'stylesheet',
          href:
            '//db.onlinewebfonts.com/c/0007c768c0c6149485a44a0409d9433c?family=GalanoGrotesque-Regular',
        },
      ],
    }
  },
}
</script>

<style scoped>
.logo-text {
  font-size: 20px;
  margin-bottom: -3px;
}
* {
  font-family: 'GalanoGrotesque-Regular', 'Quicksand', 'Source Sans Pro',
    -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, 'Helvetica Neue',
    Arial, sans-serif;
}
</style>
