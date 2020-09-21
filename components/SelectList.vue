<template>
  <div class="mt-5 mb-5">
    <div>
      <v-select
        :clearable="false"
        :close-on-select="false"
        placeholder="Use Optima to work"
        :options="useOptimaToWork"
        label="title"
      >
        <template v-slot:option="option">
          {{ option.title }}
        </template>
      </v-select>
    </div>

    <div>
      <v-select
        :close-on-select="false"
        :clearable="false"
        placeholder="Get started with Optima"
        :options="getStartedWithOptima"
        label="title"
      >
        <template v-slot:option="option">
          <a href="/userguide/optima">
            {{ option.title }}
          </a>
        </template>
      </v-select>
    </div>

    <div>
      <v-select
        :clearable="false"
        :close-on-select="false"
        placeholder="Get started with Optima"
        :options="getStartedWithOptima"
        label="title"
      >
        <template v-slot:option="option">
          <a href="/userguide/optima">
            {{ option.title }}
          </a>
        </template>
      </v-select>

      <div>
        <v-select
          :clearable="false"
          :close-on-select="false"
          placeholder="Create and personalize a profile"
          :options="createAndPersonalizeAProfle"
          label="title"
        >
        </v-select>
      </div>

      <div>
        <v-select
          :clearable="false"
          :close-on-select="false"
          placeholder="Control your safety and privacy"
          :options="controlYourSafetyAndPrivacy"
          label="title"
        >
          <template v-slot:option="option">
            {{ option.title }}
          </template>
        </v-select>
      </div>

      <div>
        <v-select
          :clearable="false"
          :close-on-select="false"
          placeholder="Change Optima settings"
          :options="changeOptimaSettings"
          label="title"
        >
          <template v-slot:option="option">
            {{ option.title }}
          </template>
        </v-select>
      </div>

      <div>
        <v-select
          :clearable="false"
          :close-on-select="false"
          placeholder="Privacy in Optima"
          :options="privacyInOptima"
          label="title"
        >
          <template v-slot:option="option">
            {{ option.title }}
          </template>
        </v-select>
      </div>

      <div>
        <v-select
          :clearable="false"
          :close-on-select="false"
          placeholder="Create and personalize a profile"
          :options="createAndPersonalizeAProfle"
          label="title"
        >
          <template v-slot:option="option">
            {{ option.title }}
          </template>
        </v-select>
      </div>
    </div>
  </div>
</template>

<script>
import VSelect from 'vue-select'
import 'vue-select/dist/vue-select.css'

export default {
  components: {
    VSelect,
  },
  data() {
    return {
      isOpen: false,
      value: '',
      //   options: ['Select option', 'label', 'touched'],
      //   options: [
      //     { name: 'Orange', value: 'orange' },
      //     { name: 'Apple', value: 'apple' },
      //     { name: 'Grape', value: 'grape' },
      //   ],
      useOptimaToWork: [],

      getStartedWithOptima: [
        {
          id: 1,
          title: 'How do i log in on the app',
          url: 'https://facebook.com',
        },
        {
          id: 2,
          title: 'Tips and Tricks of Optima',
          url: 'https://facebook.com',
        },
        {
          id: 3,
          title: 'Get started with Optima',
          url: 'https://facebook.com',
        },
        {
          id: 4,
          title: 'Get started with Optima',
          url: 'https://facebook.com',
        },
        {
          id: 5,
          title: 'How do i log in on the app',
          url: 'https://facebook.com',
        },
      ],
      createAndPersonalizeAProfle: [],
      controlYourSafetyAndPrivacy: [],
      changeOptimaSettings: [],
      privacyInOptima: [],
    }
  },
  head() {
    return {
      link: [
        {
          rel: 'stylesheet',
          href:
            'https://db.onlinewebfonts.com/c/0007c768c0c6149485a44a0409d9433c?family=GalanoGrotesque-Regular',
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
</style>
