<template>
  <div class="flex flex-wrap px-12 justify-center bg-gray-200 p-6 footer">
    <div class="flex flex-wrap mb-3 text-center w-full border-b-2">
      <div
        class="w-full sm:w-1/2 sm:text-center md:text-left md:w-1/4 lg:w-1/5 pl:w-1/5-8 mb-6 px-2"
      >
        <h6 class="font-extrabold py-2">Products</h6>
        <ul>
          <li><a href="#">Optima</a></li>
          <li><a href="#">HumanaR</a></li>
          <li><a href="#">Dome</a></li>
        </ul>
      </div>

      <div
        class="w-full sm:w-1/2 sm:text-center md:text-left md:w-1/4 lg:w-1/5 pl:w-1/5-8 mb-6 px-2"
      >
        <h6 class="font-extrabold py-2">Prices</h6>
        <ul>
          <li><a href="#">Optima</a></li>
          <li><a href="#">HumanaR</a></li>
          <li><a href="#">Dome</a></li>
        </ul>
      </div>

      <div
        class="w-full sm:w-1/2 sm:text-center md:text-left md:w-1/4 lg:w-1/5 pl:w-1/5-8 mb-6 px-2"
      >
        <h6 class="font-extrabold py-2">Partners</h6>
        <ul>
          <li><a href="#">Find a Partner</a></li>
          <li><a href="#">Become a Partner</a></li>
          <li><a href="#">Dome</a></li>
        </ul>
      </div>

      <div
        class="w-full sm:w-1/2 sm:text-center md:text-left md:w-1/4 lg:w-1/5 pl:w-1/5-8 mb-6 px-2"
      >
        <h6 class="font-extrabold py-2">Resources</h6>
        <ul>
          <li><a href="#">User Guides</a></li>
          <li><a href="#">Demos</a></li>
          <li><a href="#">Case Studies</a></li>
          <li><a href="#">Blog</a></li>
          <li><a href="#">FAQ</a></li>
          <li><a href="#">Support</a></li>
        </ul>
      </div>

      <div
        class="w-full sm:w-1/2 sm:text-center md:text-left md:w-2/4 lg:w-1/5 pl:w-1/5-8 mb-6 px-2"
      >
        <h6 class="font-extrabold py-2">Support</h6>
        <ul>
          <li><a href="#">Support@cloudenly.com</a></li>
          <li>
            <a
              target="_blank"
              href="https://api.whatsapp.com/send?phone=+2348159530070"
              ><font-awesome-icon :icon="['fab', 'whatsapp']" /> +234
              8159530070</a
            >
          </li>
          <li>
            <a href="tel:+234556655667"
              ><font-awesome-icon :icon="['fas', 'phone']" /> +234 556655667</a
            >
          </li>
        </ul>
      </div>

      <div
        class="w-full sm:w-1/2 sm:text-center md:text-left md:w-2/4 lg:w-1/5 pl:w-1/5-8 mb-6 px-2"
      >
        <h6 class="font-extrabold py-2">Products</h6>
        <ul>
          <li><a href="#">Quantum</a></li>
          <li><a href="#">Ally</a></li>
        </ul>
      </div>

      <!-- border goes in here -->

      <!-- <div class="w-full xs:w-1/4 sm:1/2 sm:text-centermd:text-left  md:w-1/4 lg:w-1/5">
        <h6 class="py-4">Subscribe</h6>
        <form action="#">
          <div class="flex items-center mb-6">
            <input
              id="inline-full-name"
              class="bg-gray-200 appearance-none border-2 border-gray-200 w-full font-extrabold py-2 px-2 text-gray-700 leading-tight focus:outline-none focus:bg-white focus:border-purple-500"
              type="text"
              placeholder="Email"
            />
            <button
              class="bg-purple-500 ml-2 hover:bg-purple-600 text-white  py-2 px-2"
              type="submit"
            >
              Submit
            </button>
          </div>
        </form>
        <p class="bottom">© Copyright 2020 - ********.com</p>
      </div> -->
    </div>
    <!-- Newsletter Button and copyight -->
    <div class="flex flex-wrap mb-3 w-full">
      <div class="w-full mb-6 px-2">
        <font-awesome-icon :icon="['fab', 'whatsapp']" /><span> </span>

        <font-awesome-icon :icon="['fab', 'twitter']" />
        <font-awesome-icon :icon="['fab', 'facebook']" />
        <font-awesome-icon :icon="['fab', 'instagram']" />
      </div>
    </div>

    <div
      class="flex flex-wrap mb-3 w-full -mt-3 xs:-px-8 sm:-px-8 md:px-2 lg:px-2"
    >
      <div class="w-full md:w-2/4 lg:w-3/4 mb-3 text-left">
        <p>
          &copy; Copyright 2020 Scelloo.com., All rights reserved. Scelloo HQ,
          Plot 16 New Creation Street, Lekki, Lagos, Nigeria<br />Terms of
          Service. Privacy Information. Security. Careers. Contact.
        </p>
      </div>
      <div class="w-full md:w-2/4 lg:w-1/4 mb-3 text-left">
        <div class="mb-1">
          <h5 class="font-bold">Subscribe to our Newsletter</h5>
          <p>Subscibe to our Newsletter. We don't Bite!</p>
        </div>
        <form action="#">
          <div class="flex items-center mb-6">
            <input
              id="inline-full-name"
              class="bg-gray-200 appearance-none border-2 border-gray-200 w-full font-extrabold py-2 px-2 text-gray-700 leading-tight focus:outline-none hover:border-blue-500 focus:bg-white focus:border-blue-500"
              type="email"
              placeholder="Enter Email"
            />
            <button
              class="bg-blue-500 ml-2 hover:bg-white hover:text-blue-500 text-white font-extrabold py-2 px-2 shadow-lg duration-200 border rounded"
              type="submit"
            >
              Submit
            </button>
          </div>
        </form>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Footer',
  head() {
    return {
      link: [
        {
          rel: 'stylesheet',
          href:
            'https://maxcdn.bootstrapcdn.com/font-awesome/4.2.0/css/font-awesome.min.css',
        },
        {
          rel: 'stylesheet',
          href:
            'https://fonts.googleapis.com/css?family=Roboto:300,400,500,700|Material+Icons',
        },
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
.footer {
  margin-top: 10em;
}

* {
  font-family: 'GalanoGrotesque-Regular';
}

p,
a {
  color: #000;
  font-size: 14px;
}
li {
  padding-top: 5px;
}
a:hover {
  color: #ddd;
}

@media (max-width: 642px) {
  .bottom {
    text-align: center;
  }
  .pl-8 {
    padding-left: 0px;
  }

  .footer {
    margin-top: 5em;
  }
}
</style>
