<template>
  <div class="home">
    <Button @button-click="bye">Button One</Button>
    <Button @button-click="hello">Button Two</Button>
  </div>
</template>

<script>
// @ is an alias to /src
import Button from "../components/Button.vue";
export default {
  name: "Home",
  components: {
    Button,
  },
  data() {
    return {
      selected: "",
    };
  },

  methods: {
    hello: function () {
      console.log("hello");
    },
    bye: function () {
      console.log("goodbye");
    },
  },
};
</script>
<style>
</style>
