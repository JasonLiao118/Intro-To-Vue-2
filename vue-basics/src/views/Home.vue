<template>
  <div class="home">
    <Button @click="bye">Button One</Button>
       <Button @click="hello">Button Two</Button>
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

computed: {
  now: function(){
  },
},

  methods: {
    hello: function () {
      alert("hello");
    },
    bye: function () {
      alert("goodbye");
    },
  },
};
</script>
<style>
</style>


