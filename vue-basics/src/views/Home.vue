<template>
  <div class="home">
  </div>
</template>

<script>
// @ is an alias to /src
import Button from "../components/Button.vue";
export default {
  name: "Home",
  components: {
  },
  data() {
    return {
      selected: "",
    };
  },

computed: {
  now: function(){
    const time = new Date
    return `${time.getHours}: ${time.getMinutes}` ;
  },
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
