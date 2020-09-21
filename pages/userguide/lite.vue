<template>
  <div>
    <UserguideHeader />
    <Banner />
    <div class="mt-8 mb-12 flex items-center justify-center">
      <nuxt-link to="/">
        <div class="font-bold rounded-lg">
          <img
            class="inline-block"
            src="~assets/cloudenlylogo.png"
            alt="cloudenlyLogo"
          />
          <h1 class="inline-block">Cloudenly</h1>
        </div>
      </nuxt-link>
    </div>

    <!-- main content -->
    <main class="container mx-auto px-12">
      <SelectList />
    </main>
  </div>
</template>

<script>
import Banner from '../../components/Banner'
import UserguideHeader from '../../components/UserguideHeader'
import SelectList from '../../components/SelectList'

export default {
  components: {
    UserguideHeader,
    Banner,
    SelectList,
  },
}
</script>

<style scoped>
* {
  font-family: 'GalanoGrotesque-Regular', 'Quicksand', 'Source Sans Pro',
    -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, 'Helvetica Neue',
    Arial, sans-serif;
}

h1 {
  font-size: 40px;
  margin-bottom: -20px;
  margin-left: -8px;
}

img {
  margin-top: -28px;
  height: 80px;
}
/* .resource-card {
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

h5 {
  margin-top: 20px;
  font-size: 14px;
  margin-bottom: 20px;
}

.userguideicons {
  width: 50%;
  margin: auto;
} */
</style>
