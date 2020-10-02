<template>
  <div>
    <Header />
    <Banner />
    <main class="container mx-auto px-10 py-10">
      <div class="flex flex-wrap">
        <!-- Row One Starts here! -->
        <div class="px-4 w-full sm:w-1/2 md:w-1/3 lg:w-1/4 xl:w-1/4 mb-4">
          <nuxt-link to="/userguide">
            <div class="resource-card bg-gray-200">
              <div class="text-center mr-3 ml-3">
                <h1 class="font-bold">User Guide</h1>
                <div style="max-width: 400px; margin: auto">
                  <p class="font-normal">
                    Start a discussion, browse solutions, and get tips from us
                  </p>
                </div>
              </div>
            </div>
          </nuxt-link>
        </div>
        <!-- Row Two Ends Here -->
        <div class="px-4 w-full sm:w-1/2 md:w-1/3 lg:w-1/4 xl:w-1/4 mb-6">
          <nuxt-link to="/">
            <div class="resource-card bg-gray-200">
              <div class="text-center mr-3 ml-3">
                <h1 class="font-bold">White Paper</h1>
                <div style="max-width: 400px; margin: auto">
                  <p class="font-normal">
                    Start a discussion, browse solutions, and get tips from us
                  </p>
                </div>
              </div>
            </div>
          </nuxt-link>
        </div>

        <div class="px-4 w-full sm:w-1/2 md:w-1/3 lg:w-1/4 xl:w-1/4 mb-6">
          <nuxt-link to="/">
            <div class="resource-card bg-gray-200">
              <div class="text-center mr-3 ml-3">
                <h1 class="font-bold">Blog</h1>
                <div style="max-width: 400px; margin: auto">
                  <p class="font-normal">
                    Start a discussion, browse solutions, and get tips from us
                  </p>
                </div>
              </div>
            </div>
          </nuxt-link>
        </div>

        <div class="px-4 w-full sm:w-1/2 md:w-1/3 lg:w-1/4 xl:w-1/4 mb-6">
          <nuxt-link to="/">
            <div class="resource-card bg-gray-200">
              <div class="text-center mr-3 ml-3">
                <h1 class="font-bold">Community</h1>
                <div style="max-width: 400px; margin: auto">
                  <p class="font-normal">
                    Start a discussion, browse solutions, and get tips from us
                  </p>
                </div>
              </div>
            </div>
          </nuxt-link>
        </div>

        <div class="px-4 w-full sm:w-1/2 md:w-1/3 lg:w-1/4 xl:w-1/4 mb-6">
          <nuxt-link to="/">
            <div class="resource-card bg-gray-200">
              <div class="text-center mr-3 ml-3">
                <h1 class="font-bold">FAQ</h1>
                <div style="max-width: 400px; margin: auto">
                  <p class="font-normal">
                    Start a discussion, browse solutions, and get tips from us
                  </p>
                </div>
              </div>
            </div>
          </nuxt-link>
        </div>

        <div class="px-4 w-full sm:w-1/2 md:w-1/3 lg:w-1/4 xl:w-1/4 mb-6">
          <nuxt-link to="/">
            <div class="resource-card bg-gray-200">
              <div class="text-center mr-3 ml-3">
                <h1 style="margin-bottom: -24px" class="font-bold">
                  Developer Documentation
                </h1>
                <div style="max-width: 400px; margin: auto">
                  <p class="font-normal">
                    Start a discussion, browse solutions, and get tips from us
                  </p>
                </div>
              </div>
            </div>
          </nuxt-link>
        </div>

        <div class="px-4 w-full sm:w-1/2 md:w-1/3 lg:w-1/4 xl:w-1/4 mb-6">
          <nuxt-link to="/">
            <div class="resource-card bg-gray-200">
              <div class="text-center mr-3 ml-3">
                <h1 class="font-bold">Events</h1>
                <div style="max-width: 400px; margin: auto">
                  <p class="font-normal">
                    Start a discussion, browse solutions, and get tips from us
                  </p>
                </div>
              </div>
            </div>
          </nuxt-link>
        </div>

        <div class="px-4 w-full sm:w-1/2 md:w-1/3 lg:w-1/4 xl:w-1/4 mb-6">
          <nuxt-link to="/">
            <div class="resource-card bg-gray-200">
              <div class="text-center mr-3 ml-3">
                <h1 class="font-bold">Academy</h1>
                <div style="max-width: 400px; margin: auto">
                  <p class="font-normal">
                    Start a discussion, browse solutions, and get tips from us
                  </p>
                </div>
              </div>
            </div>
          </nuxt-link>
        </div>
      </div>
    </main>
  </div>
</template>

<script>
import Header from '../components/Header'
import Banner from '../components/Banner'
export default {
  name: 'Resources',
  components: {
    Header,
    Banner,
  },
  head() {
    return {
      title: 'Resources',
      meta: [
        {
          hid: 'Resources',
          name: 'Cloudenly Resources',
          content:
            'Flexible pricing options, from personal projects to enterprise applications, and everything in between.',
        },
      ],
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
* {
  font-family: 'GalanoGrotesque-Regular', 'Quicksand', 'Source Sans Pro',
    -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, 'Helvetica Neue',
    Arial, sans-serif;
}
.resource-card {
  padding: 80px 6px 15px 6px;
  border-radius: 6px;
}

h1 {
  line-height: 26px;
  font-size: 22px;
  font-weight: 500;
  margin-top: -50px;
}

p {
  margin-top: 120px;
  font-size: 14px;
}
</style>
