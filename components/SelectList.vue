<template>
  <div class="mt-5 mb-5">
    <v-app>
      <div>
        <v-select
          class="custom-border border-t-2 border-l-2 border-r-2 border-gray-100"
          background-color="white"
          filled
          :items="useOptimaToWork"
          label="Use Optima to work"
          item-text="title"
          item-id="id"
          hide-details
          dense
        >
          <!-- To Add a new Icon -->
          <template v-slot:append>
            <v-icon color="primary">keyboard_arrow_down</v-icon>
          </template>

          <template slot="selection" slot-scope="data">
            <span class="bg--red">{{ data.item.title }}</span>
          </template>
        </v-select>

        <!-- 2 -->

        <v-select
          class="custom-border border-t-2 border-l-2 border-r-2 border-gray-100"
          background-color="white"
          filled
          :items="getStartedWithOptima"
          label="Get started with Optima"
          item-text="title"
          item-id="id"
          hide-details
          dense
        >
          <!-- To Add a new Icon -->
          <template v-slot:append>
            <v-icon color="primary">keyboard_arrow_down</v-icon>
          </template>

          <template slot="selection" slot-scope="data">
            {{ data.item.title }}
          </template>
        </v-select>

        <v-select
          class="custom-border border-t-2 border-l-2 border-r-2 border-gray-100"
          background-color="white"
          filled
          :items="createAndPersonalizeAProfle"
          label="Create and personalize a profile"
          item-text="title"
          item-id="id"
          hide-details
          dense
        >
          <!-- To Add a new Icon -->
          <template v-slot:append>
            <v-icon color="primary">keyboard_arrow_down</v-icon>
          </template>

          <template slot="selection" slot-scope="data">
            <span class="bg--red">{{ data.item.title }}</span>
          </template>
        </v-select>

        <v-select
          class="custom-border border-t-2 border-l-2 border-r-2 border-gray-100"
          background-color="white"
          filled
          :items="controlYourSafetyAndPrivacy"
          label="Control your Safety and Privacy"
          item-text="title"
          item-id="id"
          hide-details
          dense
        >
          <!-- To Add a new Icon -->
          <template v-slot:append>
            <v-icon color="primary">keyboard_arrow_down</v-icon>
          </template>

          <template slot="selection" slot-scope="data">
            <span class="bg--red">{{ data.item.title }}</span>
          </template>
        </v-select>

        <v-select
          class="custom-border border-t-2 border-l-2 border-r-2 border-gray-100"
          background-color="white"
          filled
          :items="changeOptimaSettings"
          label="Change Optima Settings"
          item-text="title"
          item-id="id"
          hide-details
          dense
        >
          <!-- To Add a new Icon -->
          <template v-slot:append>
            <v-icon color="primary">keyboard_arrow_down</v-icon>
          </template>

          <template slot="selection" slot-scope="data">
            <span class="bg--red">{{ data.item.title }}</span>
          </template>
        </v-select>

        <v-select
          class="custom-border border-t-2 border-l-2 border-r-2 border-gray-100"
          background-color="white"
          filled
          :items="privacyInOptima"
          label="Privacy In Optima"
          item-text="title"
          item-id="id"
          hide-details
          dense
        >
          <!-- To Add a new Icon -->
          <template v-slot:append>
            <v-icon color="primary">keyboard_arrow_down</v-icon>
          </template>

          <template slot="selection" slot-scope="data">
            <span class="bg--red">{{ data.item.title }}</span>
          </template>
        </v-select>

        <v-select
          class="custom-border border-t-2 border-l-2 border-r-2 border-b-2 border-gray-100"
          background-color="white"
          filled
          :items="createAndPersonalizeAProfle"
          label="Create and Personlize a profile"
          item-text="title"
          item-id="id"
          hide-details
          dense
        >
          <!-- To Add a new Icon -->
          <template v-slot:append>
            <v-icon color="primary">keyboard_arrow_down</v-icon>
          </template>

          <template slot="selection" slot-scope="data">
            <span class="bg--red">{{ data.item.title }}</span>
          </template>
        </v-select>
      </div>
    </v-app>
  </div>
</template>

<script>
export default {
  components: {},
  data() {
    return {
      isOpen: false,
      value: '',

      useOptimaToWork: [
        {
          id: 1,
          title: 'How do i log in on the app?',
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
          title: 'How do i log in on the app?',
          url: 'https://facebook.com',
        },
      ],

      getStartedWithOptima: [
        {
          id: 1,
          title: 'How do i log in on the app?',
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
          title: 'How do i log in on the app?',
          url: 'https://facebook.com',
        },
      ],
      createAndPersonalizeAProfle: [
        {
          id: 1,
          title: 'How do i log in on the app?',
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
          title: 'How do i log in on the app?',
          url: 'https://facebook.com',
        },
      ],
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

<style>
* {
  font-family: 'GalanoGrotesque-Regular', 'Quicksand', 'Source Sans Pro',
    -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, 'Helvetica Neue',
    Arial, sans-serif;
}

.custom-border.v-text-field > .v-input__control > .v-input__slot:before {
  border-style: none;
}
.custom-border.v-text-field > .v-input__control > .v-input__slot:after {
  border-style: none;
}
</style>
