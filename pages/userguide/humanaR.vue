<template>
  <div>
    <UserguideHeader />
    <Banner />
    <div class="mt-12 mb-8 flex items-center text-center justify-center">
      <nuxt-link to="/userguide/humanaR">
        <div class="rounded-lg">
          <img
            class="mr-3 inline-block"
            src="~assets/userguideIcons/HumanaR.png"
            alt="humanaRLogo"
          />
          <h1 class="font-bold inline-block">HumanaR</h1>
          <!-- The one below Doesnt look to Good -->
          <!-- <h2 class="-ml-24 my-3">User Guide</h2> -->
          <h3 class="-mt-2 font-semibold">User Guide</h3>
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
          heading: 'Get Started with HumanaR',
          content1: 'How do i log in on the app?',
          url1: '',
          content2: 'Tips and Tricks of HumanaR',
          url2: '',
          content3: 'Get started with HumanaR',
          url3: '',
        },
        {
          id: 2,
          heading: 'Organization',
          content1: 'Functional Hierarchy',
          url1: '',
          content2: 'Job Level',
          url2: '',
          content3: 'Designation',
          url3: '',
          content4: 'People',
          url4: '',
        },
        {
          id: 3,
          heading: 'Location and Tax',
          content1: 'Location',
          url1: '',
          content2: 'Tax',
          url2: '',
        },
        {
          id: 5,
          heading: 'Employees',
          content1: 'Employee Directory',
          url1: '',
          content2: 'Groups',
          url2: '',
          content3: 'Designation',
          url3: '',
          content4: 'Employee Engagement',
          url4: '',
        },
        {
          id: 6,
          heading: 'HR Document',
          content1: 'HR Document',
        },
        {
          id: 7,
          heading: 'Payroll',
          content1: 'Dashboard',
          url1: '',
          content2: 'Variable Earnings',
          url2: '',
          content3: 'Employees',
          url3: '',
          content4: 'Payrun',
          url4: '',
          content5: 'Promotion',
          url5: '',
          content6: 'PAYE',
          url6: '',
          content7: 'Reports',
          url7: '',
          content8: 'Payslips',
          url8: '',
        },
        {
          id: 8,
          heading: 'Benefits',
          content1: 'Leave',
          url1: '',
          content2: 'Advance and Loans',
          url2: '',
          content3: 'Allowance',
          url3: '',
          content4: 'Overtime',
          url4: '',
          content5: 'Promotion',
          url5: '',
          content6: 'Other Benefits',
          url6: '',
        },
        {
          id: 9,
          heading: 'Performance',
          content1: 'Strategic Objectives',
          url1: '',
          content2: 'Organizational KRMs',
          url2: '',
          content3: 'Agreements',
          url3: '',
          content4: 'Review',
          url4: '',
          content5: 'Improvement',
          url5: '',
        },
        {
          id: 10,
          heading: 'Employee Self-Service (EES)',
          content1: 'Employee Self-Service (EES)',
          url1: '',
        },
        {
          id: 11,
          heading: 'Settings',
          content1: 'Profile',
          url1: '',
          content2: 'Pay Settings',
          url2: '',
          content3: 'Pay Schedule',
          url3: '',
          content4: 'Pension',
          url4: '',
          content5: 'Location and Tax',
          url5: '',
          content6: 'Security',
          url6: '',
        },
      ],
    }
  },
  head() {
    return {
      title: 'HumanaR',
      meta: [
        {
          hid: 'HumanaR',
          name: 'HumanaR',
          content: 'Tips and Tricks of HumanaR, Get started with HumanaR ',
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
