<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png" />
    <!-- <HelloWorld msg="Welcome to Your Vue.js App" /> -->
    <!-- <Product :premium="premium" @change-permium="click"></Product> -->
    
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";
import Product from "@/components/Product.vue";

export default {
  name: "Home",
  components: {
    // HelloWorld,
    // Product,
  },
  data() {
    return {
    };
  },
  methods: {
    click() {},
  },
};
</script>
<style scoped>
</style>