<template>
    <a :href="link" :alt="name">
        <button class="button is-network-button is-medium is-black is-rounded">
            <span class="icon is-medium">
              <i class="fab" :class="'fa-' + logo"></i>
            </span>
            <span>{{name}}</span>
        </button>
    </a>
</template>

<script>
export default {
  name: 'Network',
  props: {
    name: String,
    logo: String,
    link: String
  },
  methods: {

  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
    button.is-network-button {
        background: black;
        transition: 0.3s;
    }
    button.is-network-button:hover {
        background: #04a5e7;
    }
</style>
