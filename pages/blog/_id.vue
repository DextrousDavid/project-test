<template>
  <div>
    <UserguideHeader />
    <div class="container">
      <div class="post">
        <h2>Hollaaa</h2>
        <h2 class="mb-8">{{ post.slug }}</h2>
      </div>
    </div>
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
        .get('https://ojreloaded.com.ng/wp-json/wp/v2/posts/' + params.id)
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
