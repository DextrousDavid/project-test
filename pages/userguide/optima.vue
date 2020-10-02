<template>
  <div>
    <UserguideHeader />
    <Banner />
    <div class="mt-12 mb-8 flex items-center text-center justify-center">
      <nuxt-link to="/userguide/optima">
        <div class="rounded-lg">
          <img
            class="mr-3 inline-block"
            src="~assets/userguideIcons/Optima1.png"
            alt="Optimalogo"
          />
          <h1 class="font-bold inline-block">Optima</h1>
          <!-- The one below Doesnt look to Good -->
          <!-- <h2 class="-ml-24 my-3">User Guide</h2> -->
          <h3 class="ml-8 -mt-2 font-semibold">User Guide</h3>
        </div>
      </nuxt-link>
    </div>

    <!-- main content -->
    <main class="container">
      <Accordion :user-guides="userGuides" />
    </main>
  </div>
</template>

<script>
import Banner from '../../components/Banner'
import UserguideHeader from '../../components/UserguideHeader'
import Accordion from '../../components/Accordion'

export default {
  components: {
    UserguideHeader,
    Banner,
    Accordion,
  },
  data() {
    return {
      userGuides: [
        {
          id: 1,
          heading: 'Get Started With Optima',
          content1: 'How do i log in on the app?',
          url1: '//facebook.com',
          content2: 'Tips and Tricks of Optima',
          url2: '',
          content3: 'Get started with Optima',
          url3: '',
        },
        {
          id: 2,
          heading: 'Customer Relationship Management (CRM)',
          content1: 'Customer Registration',
          url1:
            'https://resources.cloudenly.com/knowledge-base/customer-registration/',
          content2: 'Customer Engagement',
          url2:
            'https://resources.cloudenly.com/knowledge-base/customer-engagement/',
          content3: 'Pipeline Management',
          url3:
            'https://resources.cloudenly.com/knowledge-base/pipeline-management/',
          content4: 'Promotions',
          url4: 'https://resources.cloudenly.com/knowledge-base/promotion/',
          content5: 'Meeting',
          url5: 'https://resources.cloudenly.com/knowledge-base/meeting/',
        },
        {
          id: 3,
          heading: 'Purchase',
          content1: 'Supplier',
          url1: '',
          content2: 'Catalogue',
          url2: '',
          content3: 'Purchase Requisition',
          url3: '',
          content4: 'Request for Quote (RFQ)',
          url4: '',
          content5: 'Quote',
          url5: '',
          content6: 'Purchase Order (PO)',
          url6: '',
          content7: 'Invoice',
          url7: '',
          content8: 'Debit Note',
          url8: '',
        },
        {
          id: 4,
          heading: 'Sales',
          content1: 'Catalogue',
          url1: '',
          content2: 'Pricebook',
          url2: '',
          content3: 'Request for Quote (RFQ)',
          url3: '',
          content: 'Quote',
          url: '',
          content4: 'Purchase Order (PO)',
          url4: '',
          content5: 'Invoice',
          url5: '',
          content6: 'Waybill',
          url6: '',
          content7: 'Credit Note',
          url7: '',
        },
        {
          id: 5,
          heading: 'Inventory',
          content1: 'Outlets and Inventory Classes',
          url1: '',
          content2: 'Stock Balance',
          url2: '',
          content3: 'Waybill',
          url3: '',
          content4: 'Goods Received Note',
          url4: '',
          content5: 'Material Request',
          url5: '',
          content6: 'Material Return',
          url6: '',
        },
        {
          id: 6,
          heading: 'Production',
          content1: 'Production',
          url1: '',
        },
        {
          id: 7,
          heading: 'Finance',
          content1: 'Finance',
          url1: '',
        },
        {
          id: 8,
          heading: 'Payment',
          content1: 'Payment',
          url1: '',
        },
        {
          id: 9,
          heading: 'Accounts',
          content1: 'Accounts',
          url1: '',
        },
        {
          id: 10,
          heading: 'Approval Center',
          content1: 'Approval Center',
          url1: '',
        },
        {
          id: 11,
          heading: 'Settings',
          content1: 'Settings',
          url1: '',
        },
      ],
    }
  },
  head() {
    return {
      title: 'Optima',
      meta: [
        {
          hid: 'Optima',
          name: 'Optima',
          content: 'Tips and Tricks of Optima, Get started with Optima',
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

h1 {
  font-size: 40px;
  margin-bottom: -20px;
  margin-left: -8px;
}

h2 {
  font-size: 20px;
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
