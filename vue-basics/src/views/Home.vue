<template>
  <div class="home">
    <Button @button-click="bye">Button One</Button>
    <Button @button-click="hello">Button Two</Button>

    <Card
      v-for="destination in destinations"
      :key="destination.name"
      :title="destination.name"
      :price="destination.price"
      :image="destination.img"
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
      destinations: [
        {
          name: "Venetian Renaissance",
          International: true,
          price: 1300,
          img: "https://images.unsplash.com/photo-1498307833015-e7b400441eb8?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1528&q=80",
        },
        {
          name: "Swiss Mountain Getaway",
          International: true,
          price: 800,
          img: "https://images.unsplash.com/photo-1483728642387-6c3bdd6c93e5?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=1476&q=80",
        },
        {
          name: "Ibizan Coastal Vacation",
          International: true,
          price: 1200,
          img: "https://images.unsplash.com/photo-1547138494-97041dec734b?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=1170&q=80",
        },
        {
          name: "Hawaiian Vacation",
          International: false,
          price: 900,
          img: "https://images.unsplash.com/photo-1507525428034-b723cf961d3e?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=1173&q=80",
        },
        {
          name: "Cascade Mountains",
          International: false,
          price: 400,
          img: "https://images.unsplash.com/photo-1511497584788-876760111969?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=1332&q=80",
        },
        {
          name: "Egyptian Exploration",
          International: true,
          price: 800,
          img: "https://images.unsplash.com/photo-1473580044384-7ba9967e16a0?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1170&q=80",
        },
      ],
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
