<template>
  <div class="home">
    <Button @button-click="bye">Button One</Button>
    <Button @button-click="hello">Button Two</Button>
    <Card
      title="Hello World"
      description="When used to bind the class or style attribute, it supports additional value types such as Array or Objects. See linked guide section below for more details."
      image="https://cdn.pixabay.com/photo/2021/12/11/07/59/hotel-6862159_960_720.jpg"
    />
  </div>
</template>

<script>
// @ is an alias to /src
import Button from "../components/Button.vue";
import Card from "../components/Card.vue";

export default {
  name: "Home",
  components: {
    Button,
    Card,
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
