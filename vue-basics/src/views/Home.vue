<template>
  <div class="home">
    <select v-model="selected">
      <option>A</option>
      <option>B</option>
      <option>C</option>
    </select>
    <span>{{ selected }}</span>
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: "Home",
  components: {},
  data() {
    return {
      selected: "",
    };
  },
  methods: {},
};
</script>
<style>
button {
  font-size: 30px;
}
</style>
