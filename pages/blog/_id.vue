<template>
  <div>
    <UserguideHeader />
    <section class="banner mb-2">
      <div class="mr-3 ml-3">
        <h1 class="font-normal container">Cloudenly User Guide</h1>
        <div style="max-width: 550px; margin: auto">
          <!-- <p class="font-normal">
            Flexible pricing options, from personal projects to enterprise
            applications, and everything in between
          </p> -->
        </div>
      </div>
    </section>
    <section class="container">
      <h1 class="post-title font-bold mb-1 ml-2">{{ post.title.rendered }}</h1>
      <div class="flex mb-4 -mx-2">
        <div class="main-content w-3/4 px-4">
          <p class="text-justify">{{ post.content.rendered }}</p>
        </div>

        <div class="w-1/4 px-4">
          <nuxt-link
            to="/userguide"
            class="inline-block text-sm px-3 py-3 leading-none border rounded text-white bg-blue-500 hover:bg-white hover:text-blue-500 mt-4 mb-4 lg:mt-0 shadow-md duration-200"
          >
            Read More User Guides
          </nuxt-link>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
import axios from 'axios'
import UserguideHeader from '../../components/UserguideHeader'

export default {
  components: {
    UserguideHeader,
  },
  async asyncData({ params, payload }) {
    if (payload) {
      return {
        post: payload,
      }
    } else {
      return await axios
        .get('https://resources.cloudenly.com/wp-json/wp/v2/ht_kb/' + params.id)
        .then((res) => {
          return {
            post: res.data,
          }
        })
    }
  },
  data() {
    return {
      post: {},
    }
  },
}
</script>

<style scoped>
.banner {
  max-width: 100%;
  padding: 20px 0;
  background-image: linear-gradient(269.56deg, #47c9fa 15.32%, #4881da 79.59%);
  background-repeat: no-repeat;
  background-size: 100% 100%;
  color: white;
}

h1 {
  font-size: 20px;
}

.post-title {
  font-size: 30px;
}

i.v-icon.v-icon {
  color: white;
}
</style>
