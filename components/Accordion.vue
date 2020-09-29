<template>
  <div class="mt-3">
    <v-app>
      <div class="xs:px-16 sm:px-16 md:mx-40 lg:mx-48">
        <v-expansion-panels accordion hover>
          <v-expansion-panel>
            <v-expansion-panel-header>
              Get started with Optima
              <template v-slot:actions>
                <v-icon color="primary">$expand</v-icon>
              </template>
            </v-expansion-panel-header>

            <div class="hover:bg-gray-500">
              <v-expansion-panel-content
                v-for="getStartedWithOptima in getStartedWithOptimas"
                :key="getStartedWithOptima.id"
                color="blue-grey lighten-5"
                hover
              >
                <nuxt-link
                  :to="{
                    name: 'blog-id',
                    params: { id: posts.id, slug: posts.slug },
                  }"
                >
                  <div style="color: #4242be">
                    {{ getStartedWithOptima.title }}
                  </div>
                </nuxt-link>
              </v-expansion-panel-content>
            </div>
          </v-expansion-panel>

          <v-expansion-panel>
            <v-expansion-panel-header>
              Customer Relationship Management (CRM)
              <template v-slot:actions>
                <v-icon color="primary">$expand</v-icon>
              </template>
            </v-expansion-panel-header>

            <v-expansion-panel-content
              v-for="crm in crms"
              :key="crm.id"
              color="blue-grey lighten-5"
            >
              <a :href="crm.url">
                {{ crm.title }}
              </a>
            </v-expansion-panel-content>
          </v-expansion-panel>

          <v-expansion-panel>
            <v-expansion-panel-header>
              Purchase
              <template v-slot:actions>
                <v-icon color="primary">$expand</v-icon>
              </template>
            </v-expansion-panel-header>

            <v-expansion-panel-content
              v-for="purchase in purchases"
              :key="purchase.id"
              color="blue-grey lighten-5"
            >
              <nuxt-link to="/">
                <div style="color: #000">{{ purchase.title }}</div>
              </nuxt-link>
            </v-expansion-panel-content>
          </v-expansion-panel>

          <v-expansion-panel>
            <v-expansion-panel-header>
              Sales
              <template v-slot:actions>
                <v-icon color="primary">$expand</v-icon>
              </template>
            </v-expansion-panel-header>

            <v-expansion-panel-content
              v-for="sale in sales"
              :key="sale.id"
              color="blue-grey lighten-5"
            >
              <nuxt-link to="/">
                <div style="color: #000">{{ sale.title }}</div>
              </nuxt-link>
            </v-expansion-panel-content>
          </v-expansion-panel>

          <v-expansion-panel>
            <v-expansion-panel-header>
              Inventory
              <template v-slot:actions>
                <v-icon color="primary">$expand</v-icon>
              </template>
            </v-expansion-panel-header>

            <v-expansion-panel-content
              v-for="inventory in inventories"
              :key="inventory.id"
              color="blue-grey lighten-5"
            >
              <nuxt-link to="/">
                <div style="color: #000">{{ inventory.title }}</div>
              </nuxt-link>
            </v-expansion-panel-content>
          </v-expansion-panel>

          <v-expansion-panel>
            <v-expansion-panel-header>
              Production
              <template v-slot:actions>
                <v-icon color="primary">$expand</v-icon>
              </template>
            </v-expansion-panel-header>

            <v-expansion-panel-content
              v-for="production in productions"
              :key="production.id"
              color="blue-grey lighten-5"
            >
              <nuxt-link to="/">
                <div style="color: #000">{{ production.title }}</div>
              </nuxt-link>
            </v-expansion-panel-content>
          </v-expansion-panel>

          <v-expansion-panel>
            <v-expansion-panel-header>
              Finance
              <template v-slot:actions>
                <v-icon color="primary">$expand</v-icon>
              </template>
            </v-expansion-panel-header>

            <v-expansion-panel-content
              v-for="finance in finances"
              :key="finance.id"
              color="blue-grey lighten-5"
            >
              <nuxt-link to="/">
                <div style="color: #000">{{ finance.title }}</div>
              </nuxt-link>
            </v-expansion-panel-content>
          </v-expansion-panel>

          <v-expansion-panel>
            <v-expansion-panel-header>
              Payment
              <template v-slot:actions>
                <v-icon color="primary">$expand</v-icon>
              </template>
            </v-expansion-panel-header>

            <v-expansion-panel-content
              v-for="payment in payments"
              :key="payment.id"
              color="blue-grey lighten-5"
            >
              <nuxt-link to="/">
                <div style="color: #000">{{ payment.title }}</div>
              </nuxt-link>
            </v-expansion-panel-content>
          </v-expansion-panel>

          <v-expansion-panel>
            <v-expansion-panel-header>
              Accounts
              <template v-slot:actions>
                <v-icon color="primary">$expand</v-icon>
              </template>
            </v-expansion-panel-header>

            <v-expansion-panel-content
              v-for="account in accounts"
              :key="account.id"
              color="blue-grey lighten-5"
            >
              <nuxt-link to="/">
                <div style="color: #000">{{ account.title }}</div>
              </nuxt-link>
            </v-expansion-panel-content>
          </v-expansion-panel>

          <v-expansion-panel>
            <v-expansion-panel-header>
              Approval Center
              <template v-slot:actions>
                <v-icon color="primary">$expand</v-icon>
              </template>
            </v-expansion-panel-header>

            <v-expansion-panel-content
              v-for="approvalcenter in approvalcenters"
              :key="approvalcenter.id"
              color="blue-grey lighten-5"
            >
              <nuxt-link to="/">
                <div style="color: #000">{{ approvalcenter.title }}</div>
              </nuxt-link>
            </v-expansion-panel-content>
          </v-expansion-panel>

          <v-expansion-panel>
            <v-expansion-panel-header>
              Settings
              <template v-slot:actions>
                <v-icon color="primary">$expand</v-icon>
              </template>
            </v-expansion-panel-header>

            <v-expansion-panel-content
              v-for="setting in settings"
              :key="setting.id"
              color="blue-grey lighten-5"
            >
              <nuxt-link to="/">
                <div style="color: #000">{{ setting.title }}</div>
              </nuxt-link>
            </v-expansion-panel-content>
          </v-expansion-panel>
        </v-expansion-panels>
      </div>
    </v-app>
  </div>
</template>

<script>
import axios from 'axios'

export default {
  components: {},
  fetch({ store }) {
    return axios
      .get('https://resources.cloudenly.com/wp-json/wp/v2/ht_kb/')
      .then((res) => {
        store.commit('frontPagePosts', res.data)
      })
  },
  data() {
    return {
      isOpen: false,
      value: '',

      crms: [
        {
          id: 1,
          title: 'Customer Registration',
          url:
            'https://resources.cloudenly.com/knowledge-base/customer-registration/',
        },
        {
          id: 2,
          title: 'Customer Engagement',
          url:
            'https://resources.cloudenly.com/knowledge-base/customer-engagement/',
        },
        {
          id: 3,
          title: 'Pipeline Management',
          url:
            'https://resources.cloudenly.com/knowledge-base/pipeline-management/',
        },
        {
          id: 4,
          title: 'Promotions',
          url: 'https://resources.cloudenly.com/knowledge-base/promotion/',
        },
        {
          id: 5,
          title: 'Meeting',
          url: 'https://resources.cloudenly.com/knowledge-base/meeting/',
        },
      ],

      getStartedWithOptimas: [
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
      ],
      purchases: [
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
      inventories: [
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
      privacyInOptimas: [],
      productions: [],
      finances: [],
      payments: [],
      accounts: [],
      approvalcenters: [],
      settings: [],
    }
  },
  computed: {
    posts() {
      return this.$store.state.posts
    },
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
.v-expansion-panel::before {
  outline: none !important;
}

.v-expansion-panel-header {
  outline: none !important;
  font-weight: 500;
}
</style>
