<template>
  <form class="example" style="margin-top: 30px">
    <div
      style="max-width: 500px; margin: auto"
      class="flex items-center flex-shrink-0 justify-between mb-10 focus:outline-none outline-none"
    >
      <v-text-field placeholder="Describe your issue..." solo>
        <template v-slot:append>
          <v-btn icon color="success">
            <i class="fa fa-search fa-lg" aria-hidden="true"></i>
            <!-- <i class="fa fa-search" aria-hidden="true"></i> -->
          </v-btn>
        </template>
      </v-text-field>
      <!-- <button
        class="inline-block w-20 pt-2 py-2 px-2 border-none appearance-none focus:outline-none outline-none"
        type="submit"
      >
        
      </button>
      <input
        class="inline-block bg-white outline-none focus:outline-none appearance-none border border-white w-full py-3 px-2 text-gray-700 pt-3 leading-tight"
        type="text"
        placeholder="Describe your issue..."
      /> -->
    </div>
  </form>
</template>

<script>
export default {
  name: 'Inputform',
  head() {
    return {
      link: [
        {
          rel: 'stylesheet',
          href:
            'https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css',
        },
      ],
    }
  },
}
</script>

<style>
* {
  box-sizing: border-box;
}

i {
  color: rgb(59, 178, 226);
  padding-left: 10px;
  margin-left: -20px;
}

i.v-icon.v-icon {
  color: blue;
}

v-btn {
  color: red;
}
</style>
