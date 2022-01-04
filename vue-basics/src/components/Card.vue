<template>
  <div class="card">
    <h2>{{ title }}</h2>
    <img :src="getImage" alt="" />
    <h3>{{ price }}</h3>
  </div>
</template>

<script>
export default {
  name: "Card",
  props: {
    title: String,
    price: Number,
    image: String,
  },
  computed: {
    getImage: function () {
      return this.image;
    },
  },
};
</script>

<style >
.card {
  width: 30%;
  background-color: red;
  height: 500px;
  margin: 10px auto;
}
img {
  width: 100%;
}
</style>