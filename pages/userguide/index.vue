<template>
  <div>
    <!-- Banner goes in here -->
    <UserguideHeader />
    <Banner />
    <div class="mt-10 mb-4 flex items-center justify-center">
      <nuxt-link to="/">
        <div class="font-extrabold rounded-lg">
          <img
            class="img-logo inline-block"
            src="~assets/cloudenlylogo.png"
            alt="cloudenlyLogo"
          />
          <h1 class="font-extrabold h1-logo inline-block">Cloudenly</h1>
        </div>
      </nuxt-link>
    </div>

    <!-- main content -->
    <main class="container mx-auto px-10 py-10">
      <div class="flex flex-wrap -mx-2">
        <!-- Row One Starts here! -->
        <div class="px-4 w-full sm:w-1/2 md:w-1/3 lg:w-1/4 xl:w-1/4 mb-4">
          <nuxt-link to="/userguide/optima">
            <div class="resource-card shadow-md">
              <div class="text-center mr-3 ml-3">
                <!-- <h1 class="font-bold">User Guide</h1> -->
                <div style="max-width: 400px; margin: auto">
                  <img
                    class="userguideicons"
                    src="~assets/userguideIcons/Optima1.png"
                    alt="optima1"
                  />
                  <h5 class="font-semibold">Optima</h5>
                </div>
              </div>
            </div>
          </nuxt-link>
        </div>
        <!-- Row 1 Ends Here -->
        <div class="px-4 w-full sm:w-1/2 md:w-1/3 lg:w-1/4 xl:w-1/4 mb-4">
          <nuxt-link to="/userguide/humanaR">
            <div class="resource-card shadow-md">
              <div class="text-center mr-3 ml-3">
                <!-- <h1 class="font-bold">User Guide</h1> -->
                <div style="max-width: 400px; margin: auto">
                  <img
                    class="userguideicons"
                    src="~assets/userguideIcons/HumanaR.png"
                    alt="humanaR"
                  />
                  <h5 class="font-semibold">HumanaR</h5>
                </div>
              </div>
            </div>
          </nuxt-link>
        </div>

        <div class="px-4 w-full sm:w-1/2 md:w-1/3 lg:w-1/4 xl:w-1/4 mb-4">
          <nuxt-link to="/userguide/dome">
            <div class="resource-card shadow-md">
              <div class="text-center mr-3 ml-3">
                <!-- <h1 class="font-bold">User Guide</h1> -->
                <div style="max-width: 400px; margin: auto">
                  <img
                    class="userguideicons"
                    src="~assets/userguideIcons/Dome.png"
                    alt="Dome"
                  />
                  <h5 class="font-semibold">Dome</h5>
                </div>
              </div>
            </div>
          </nuxt-link>
        </div>

        <div class="px-4 w-full sm:w-1/2 md:w-1/3 lg:w-1/4 xl:w-1/4 mb-4">
          <nuxt-link to="/userguide/ally">
            <div class="resource-card shadow-md">
              <div class="text-center mr-3 ml-3">
                <!-- <h1 class="font-bold">User Guide</h1> -->
                <div style="max-width: 400px; margin: auto">
                  <img
                    class="userguideicons"
                    src="~assets/userguideIcons/Ally.png"
                    alt="Ally"
                  />
                  <h5 class="font-semibold">Ally</h5>
                </div>
              </div>
            </div>
          </nuxt-link>
        </div>

        <div class="px-4 w-full sm:w-1/2 md:w-1/3 lg:w-1/4 xl:w-1/4 mb-4">
          <nuxt-link to="/userguide/quantum">
            <div class="resource-card shadow-md">
              <div class="text-center mr-3 ml-3">
                <!-- <h1 class="font-bold">User Guide</h1> -->
                <div style="max-width: 400px; margin: auto">
                  <img
                    class="userguideicons"
                    src="~assets/userguideIcons/Quantum.png"
                    alt="Quantum"
                  />
                  <h5 class="font-semibold">Quantum</h5>
                </div>
              </div>
            </div>
          </nuxt-link>
        </div>

        <div class="px-4 w-full sm:w-1/2 md:w-1/3 lg:w-1/4 xl:w-1/4 mb-4">
          <nuxt-link to="/userguide/lite">
            <div class="resource-card shadow-md">
              <div class="text-center mr-3 ml-3">
                <!-- <h1 class="font-bold">User Guide</h1> -->
                <div style="max-width: 400px; margin: auto">
                  <img
                    class="userguideicons"
                    src="~assets/userguideIcons/Lite.png"
                    alt="Lite"
                  />
                  <h5 class="font-semibold">Lite</h5>
                </div>
              </div>
            </div>
          </nuxt-link>
        </div>

        <div class="px-4 w-full sm:w-1/2 md:w-1/3 lg:w-1/4 xl:w-1/4 mb-4">
          <nuxt-link to="/userguide/humanaR">
            <div class="resource-card shadow-md">
              <div class="text-center mr-3 ml-3">
                <!-- <h1 class="font-bold">User Guide</h1> -->
                <div style="max-width: 400px; margin: auto">
                  <img
                    class="userguideicons"
                    src="~assets/userguideIcons/Optima3.png"
                    alt="optima3"
                  />
                  <h5 class="font-semibold">HumanaR</h5>
                </div>
              </div>
            </div>
          </nuxt-link>
        </div>

        <div class="px-4 w-full sm:w-1/2 md:w-1/3 lg:w-1/4 xl:w-1/4 mb-4">
          <nuxt-link to="/userguide/optima">
            <div class="resource-card shadow-md">
              <div class="text-center mr-3 ml-3">
                <!-- <h1 class="font-bold">User Guide</h1> -->
                <div style="max-width: 400px; margin: auto">
                  <img
                    class="userguideicons"
                    src="~assets/userguideIcons/Optima4.png"
                    alt="optima4"
                  />
                  <h5 class="font-semibold">Optima</h5>
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
import UserguideHeader from '../../components/UserguideHeader'
import Banner from '../../components/Banner'

export default {
  components: {
    UserguideHeader,
    Banner,
  },
  head() {
    return {
      title: 'User Guide',
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
  padding: 40px 6px 15px 6px;
  border-radius: 6px;
  border: 2px solid #f4f4f4;
  margin-bottom: 40px;
}

h1 {
  line-height: 26px;
  font-size: 22px;
  font-weight: 500;
  margin-top: -50px;
}

.h1-logo {
  font-size: 40px;
  margin-bottom: -20px;
  font-weight: 900;
  margin-left: -5px;
}

.img-logo {
  margin-top: -28px;
  height: 80px;
}
h5 {
  margin-top: 20px;
  font-size: 14px;
  margin-bottom: 20px;
}

.userguideicons {
  width: 50%;
  margin: auto;
}
</style>
