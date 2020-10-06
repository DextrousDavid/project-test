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
          <h3 class="-ml-5 -mt-2 font-semibold">User Guide</h3>
        </div>
      </nuxt-link>
    </div>

    <!-- main content -->
    <main>
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
          content1: 'Organization',
          url1: '',
          content2: 'Functional Hierarchy',
          url2:
            'https://resources.cloudenly.com/knowledge-base/functional-hierarchy/',
          content3: 'Job Level',
          url3: 'https://resources.cloudenly.com/knowledge-base/job-level/',
          content4: 'Designation',
          url4: 'https://resources.cloudenly.com/knowledge-base/designation/',
          content5: 'People',
          url5: 'https://resources.cloudenly.com/knowledge-base/people/',
        },
        {
          id: 3,
          heading: 'Location and Tax',
          content1: 'Location and Tax',
          url1: 'https://resources.cloudenly.com/knowledge-base/location/',
          content2: 'Location',
          url2: 'https://resources.cloudenly.com/knowledge-base/location/',
          content3: 'Tax',
          url3: 'https://resources.cloudenly.com/knowledge-base/location/',
        },
        {
          id: 5,
          heading: 'Employees',
          content1: 'Employees',
          url1:
            'https://resources.cloudenly.com/knowledge-base/humanar-employees/',
          content2: 'Employee Directory',
          url2:
            'https://resources.cloudenly.com/knowledge-base/humanar-employee-directory/',
          content3: 'Groups',
          url3:
            'https://resources.cloudenly.com/knowledge-base/employee-groups/',
          content4: 'Designation',
          url4: 'https://resources.cloudenly.com/knowledge-base/designation/',
          content5: 'Employee Engagement',
          url5:
            'https://resources.cloudenly.com/knowledge-base/employee-engagement/',
        },
        {
          id: 6,
          heading: 'HR Document',
          content1: 'HR Document',
          url1: 'https://resources.cloudenly.com/knowledge-base/hr-document/',
        },
        {
          id: 7,
          heading: 'Payroll',
          content1: 'Payroll',
          url1:
            'https://resources.cloudenly.com/knowledge-base/payroll-dashboard/',
          content2: 'Dashboard',
          url2:
            'https://resources.cloudenly.com/knowledge-base/payroll-dashboard/',
          content3: 'Variable Earnings',
          url3: '',
          content4: 'Employees',
          url4:
            'https://resources.cloudenly.com/knowledge-base/humanar-employees/',
          content5: 'Payrun',
          url5: '',
          content6: 'Promotion',
          url6: 'https://resources.cloudenly.com/knowledge-base/promotion/',
          content7: 'PAYE',
          url7: '',
          content8: 'Reports',
          url8: '',
          content9: 'Payslips',
          url9: '',
        },
        {
          id: 8,
          heading: 'Benefits',
          content1: 'Benefits',
          url1: 'https://resources.cloudenly.com/knowledge-base/benefits/',
          content2: 'Leave',
          url2: 'https://resources.cloudenly.com/knowledge-base/leave/',
          content3: 'Advance and Loans',
          url3: '',
          content4: 'Allowance',
          url4: '',
          content5: 'Overtime',
          url5: '',
          content6: 'Promotion',
          url6: 'https://resources.cloudenly.com/knowledge-base/promotion/',
          content7: 'Other Benefits',
          url7: 'https://resources.cloudenly.com/knowledge-base/benefits/',
        },
        {
          id: 9,
          heading: 'Performance',
          content1: 'Performance',
          url1: '',
          content2: 'Strategic Objectives',
          url2: '',
          content3: 'Organizational KRMs',
          url3: '',
          content4: 'Agreements',
          url4: '',
          content5: 'Review',
          url5: '',
          content6: 'Improvement',
          url6: '',
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
          content1: 'Settings',
          url1: 'https://resources.cloudenly.com/knowledge-base/settings/',
          content2: 'Profile',
          url2: 'https://resources.cloudenly.com/knowledge-base/profile/',
          content3: 'Pay Settings',
          url3: 'https://resources.cloudenly.com/knowledge-base/pay-setting/',
          content4: 'Pay Schedule',
          url4: 'https://resources.cloudenly.com/knowledge-base/pay-schedule/',
          content5: 'Pension',
          url5:
            'https://resources.cloudenly.com/knowledge-base/pension-setting/',
          content6: 'Location and Tax',
          url6: 'https://resources.cloudenly.com/knowledge-base/location/',
          content7: 'Security',
          url7: 'https://resources.cloudenly.com/knowledge-base/security/',
        },
      ],
    }
  },
  head() {
    return {
      title: 'HumanaR - User Guide',
      meta: [
        {
          hid: 'HumanaR - User Guide',
          name: 'HumanaR - User Guide',
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
