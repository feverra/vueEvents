<template>
  <div>{{ premium }}</div>
  <button @click="click">Click</button>
</template>

<script>
export default {
  props: {
    premium: {
      type: Boolean,
      required: true,
    },
  },
  methods: {
    click() {
      //   this.premium = !this.premium;
      this.$emit("change-permium", this.premium);
    },
  },
};
</script>

<style>
</style>