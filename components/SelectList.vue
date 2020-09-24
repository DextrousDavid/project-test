<template>
  <div class="mt-3 mb-5">
    <v-app>
      <div class="xs:w-full sm:w-full md:mx-24 lg:mx-40">
        <v-select
          class="custom-border border-t-2 border-l-2 border-r-2 border-gray-200"
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
          class="custom-border border-t-2 border-l-2 border-r-2 border-gray-200"
          background-color="white"
          filled
          :items="crm"
          label="Customer relationship management (CRM)"
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
          class="custom-border border-t-2 border-l-2 border-r-2 border-gray-200"
          background-color="white"
          filled
          :items="purchase"
          label="Purchase"
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
          class="custom-border border-t-2 border-l-2 border-r-2 border-gray-200"
          background-color="white"
          filled
          :items="sales"
          label="Sales"
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
          class="custom-border border-t-2 border-l-2 border-r-2 border-gray-200"
          background-color="white"
          filled
          :items="inventory"
          label="Inventory"
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
          class="custom-border border-t-2 border-l-2 border-r-2 border-gray-200"
          background-color="white"
          filled
          :items="production"
          label="Production"
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
          class="custom-border border-t-2 border-l-2 border-r-2 border-gray-200"
          background-color="white"
          filled
          :items="finance"
          label="Finance"
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
            <span>{{ data.item.title }}</span>
          </template>
        </v-select>

        <v-select
          class="custom-border border-t-2 border-l-2 border-r-2 border-gray-200"
          background-color="white"
          filled
          :items="payment"
          label="Payment"
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
          class="custom-border border-t-2 border-l-2 border-r-2 border-gray-200"
          background-color="white"
          filled
          :items="accounts"
          label="Accounts"
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
          class="custom-border border-t-2 border-l-2 border-r-2 border-gray-200"
          background-color="white"
          filled
          :items="approvalCenter"
          label="Approval Center"
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
          class="custom-border border-t-2 border-b-2 border-l-2 border-r-2 border-gray-200 rounded-b-lg"
          background-color="white"
          filled
          :items="settings"
          label="Settings"
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

      crm: [
        {
          id: 1,
          title: 'Customer Registration',
          url: 'https://facebook.com',
        },
        {
          id: 2,
          title: 'Customer Engagement',
          url: 'https://facebook.com',
        },
        {
          id: 3,
          title: 'Pipeline Management',
          url: 'https://facebook.com',
        },
        {
          id: 4,
          title: 'Promotions',
          url: 'https://facebook.com',
        },
        {
          id: 5,
          title: 'Meeting',
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
      purchase: [
        {
          id: 1,
          title: 'Supplier',
          url: 'https://facebook.com',
        },
        {
          id: 2,
          title: 'Catalogue',
          url: 'https://facebook.com',
        },
        {
          id: 3,
          title: 'Purchase Requistion (PR)',
          url: 'https://facebook.com',
        },
        {
          id: 4,
          title: 'Request for Quote (RFQ)',
          url: 'https://facebook.com',
        },
        {
          id: 5,
          title: 'Quote',
          url: 'https://facebook.com',
        },
        {
          id: 6,
          title: 'Purchase Order (PO)',
          url: 'https://facebook.com',
        },
        {
          id: 7,
          title: 'Invoice',
          url: 'https://facebook.com',
        },
        {
          id: 8,
          title: 'Debit Note',
          url: 'https://facebook.com',
        },
      ],
      sales: [
        {
          id: 1,
          title: 'Catalogue',
          url: 'https://facebook.com',
        },
        {
          id: 2,
          title: 'Pricebook',
          url: 'https://facebook.com',
        },
        {
          id: 3,
          title: 'Request for Quote (RFQ)',
          url: 'https://facebook.com',
        },
        {
          id: 5,
          title: 'Quote',
          url: 'https://facebook.com',
        },
        {
          id: 6,
          title: 'Purchase Order (PO)',
          url: 'https://facebook.com',
        },
        {
          id: 7,
          title: 'Invoice',
          url: 'https://facebook.com',
        },
        {
          id: 8,
          title: 'Waybill',
          url: 'https://facebook.com',
        },
        {
          id: 8,
          title: 'Credit Note',
          url: 'https://facebook.com',
        },
      ],
      inventory: [
        {
          id: 1,
          title: 'Outlets and Inventory Classes',
          url: 'https://facebook.com',
        },
        {
          id: 2,
          title: 'Stock Balance',
          url: 'https://facebook.com',
        },
        {
          id: 3,
          title: 'Waybill',
          url: 'https://facebook.com',
        },
        {
          id: 4,
          title: 'Goods Received Note',
          url: 'https://facebook.com',
        },
        {
          id: 5,
          title: 'Material Request',
          url: 'https://facebook.com',
        },
        {
          id: 6,
          title: 'Material Return',
          url: 'https://facebook.com',
        },
      ],
      privacyInOptima: [],
      production: [],
      finance: [],
      payment: [],
      accounts: [],
      approvalCenter: [],
      settings: [],
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
