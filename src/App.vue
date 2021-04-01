<template>
  <div class="menu">
    <a v-for="(menu, index) in menus" :key="index" href="">{{ menu }}</a>
  </div>
  <div v-for="(item, index) in products" :key="index + item">
    <h4>{{ index }} : {{ item }}</h4>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      menus: ["HOME", "SHOP", "ABOUT"],
      products: ["a", "b", "c"],
    };
  },
  components: {},
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  /* margin-top: 60px; */
}

.menu {
  background: darkslateblue;
  padding: 15px;
  border-radius: 5px;
}

.menu a {
  color: white;
  padding: 10px;
}
</style>
