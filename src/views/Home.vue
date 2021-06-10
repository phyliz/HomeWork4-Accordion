<template>
  <div class="home">
    <button @click="transition()">アコーディオン</button>
  </div>
</template>

<script>
export default {
  methods: {
    transition() {
      this.$router.push({ name: "About"});
    }
  }
};
</script>

<style scoped>
.home button {
  width: 500px;
  height: 80px;
  font-size: 18px;
  text-align: left;
}
</style>