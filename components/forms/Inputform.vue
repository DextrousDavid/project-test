<template>
  <form class="example" style="margin-top: 30px">
    <div class="mb-10" style="max-width: 550px; margin: auto">
      <button type="submit">
        <i class="fa fa-search"></i>
      </button>
      <input type="text" placeholder="Describe your issue" name="search" />
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
  padding: 10px;
  font-size: 17px;
  float: left;
  width: 80%;
  color: #000;
  background: #fff;
  border-bottom-right-radius: 5px;
  outline: none;
  border: none;
}

/* Style the submit button */
form.example button {
  float: left;
  width: 20%;
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
