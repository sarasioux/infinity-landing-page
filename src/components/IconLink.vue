<template>
  <a :href="link" target="_new" :alt="alt">
    <button class="button is-large">
    <span class="icon is-medium">
      <i :class="'fa-' + icon" class="fab fa-2x"></i>
    </span>
    </button>
  </a>
</template>

<script>

  import '@fortawesome/fontawesome-free/css/all.css'

  export default {
    name: 'IconLink',
    props: {
      icon: String,
      link: String,
      alt: String
    },
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  a {
    color: black;
    transition: 0.3s;
  }
  a:hover {
    color: pink;
  }
  button {
    border: 0;
    background: transparent;
    color: black;
    transition: 0.3s;
    margin: 0 1%;
  }
  button:hover {
    color: pink;
  }
</style>
