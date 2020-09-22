<template>
  <form class="example" style="margin-top: 30px">
    <div
      style="max-width: 400px; margin: auto"
      class="flex items-center flex-shrink-0 justify-between mb-10"
    >
      <button class="inline-block" type="submit">
        <i class="fa fa-search" />
      </button>
      <input
        class="inline-block bg-white appearance-none border-2 border-gray-200 w-full font-extrabold py-3 px-2 text-gray-700 leading-tight focus:outline-none"
        type="text"
        placeholder="Enter Email"
      />
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

<style scoped>
* {
  box-sizing: border-box;
}

/* Style the search field */
form.example input[type='text'] {
  padding: 12px;
  font-size: 17px;
  color: #000;
  background: #fff;
  border-bottom-right-radius: 5px;
  outline: none;
  border: none;
  border-top-style: hidden;
  border-left-style: hidden;
}

/* Style the submit button */
form.example button {
  margin-right: -10px;
  padding: 10px;
  background: #fff;
  color: #48b6f2;
  font-size: 17px;
  border-left: none; /* Prevent double borders */
  border-top-left-radius: 5px;
  border-bottom-left-radius: 5px;
  cursor: pointer;
  outline: none;
  border: none;
}

/* Clear floats */
form.example::after {
  content: '';
  clear: both;
  display: table;
}
</style>
