<template>
  <div>
    <UserguideHeader />
    <Banner />
    <div class="mt-12 mb-8 flex items-center text-center justify-center">
      <nuxt-link to="/userguide/ally">
        <div class="rounded-lg">
          <img
            class="mr-3 inline-block"
            src="~assets/userguideIcons/Ally.png"
            alt="AllyLogo"
          />
          <h1 class="font-bold inline-block">Ally</h1>
          <h3 class="-mt-2 font-semibold">User Guide</h3>
        </div>
      </nuxt-link>
    </div>

    <!-- main content -->
    <main class="sm:container mx-auto">
      <!-- <Accordion /> -->
    </main>
  </div>
</template>

<script>
// import axios from 'axios'
import Banner from '../../components/Banner'
import UserguideHeader from '../../components/UserguideHeader'
// // import Accordion from '../../components/Accordion'
export default {
  components: {
    UserguideHeader,
    Banner,
    // Accordion,
  },
  head() {
    return {
      title: 'Ally - User Guide',
      meta: [
        {
          hid: 'Ally - User Guide',
          name: 'Ally - User Guide',
          content: 'Tips and Tricks of Ally, Get started with Ally',
        },
      ],
    }
  },

  // fetch({ store }) {
  //   return axios
  //     .get('https://resources.cloudenly.com/wp-json/wp/v2/ht_kb/144')
  //     .then((res) => {
  //       store.commit('frontPagePosts', res.data)
  //     })
  // },
  // computed: {
  //   posts() {
  //     return this.$store.state.posts
  //   },
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
  margin-left: -6px;
}

h2 {
  font-size: 20px;
}

h3 {
  margin-left: 6.7rem;
}
img {
  margin-top: -28px;
  height: 80px;
}

.v-application--wrap {
  min-height: 1vh;
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
