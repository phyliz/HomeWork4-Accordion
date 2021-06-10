<template>
  <div class="about">
    <button @click="transition()">アコーディオン</button>
    <p>アコーディオンの中身が入ります</p>
  </div>
</template>

<script>
export default {
  methods: {
    transition() {
      this.$router.push({ name: "Home" });
    }
  }
};
</script>

<style scoped>
div {
  display: block;
}
.about button,
.about p {
  width: 500px;
  height: 80px;
  border: solid 1px;
  border-radius: 0;
}
.about button {
  border-bottom: 0;
  text-align: left;
  font-size: 18px;
}
.about p {
  border-top: 0;
  align-items: center;
  font-size: 16px;
  margin-top: 0;
  padding: 25px;
  box-sizing: border-box;
}
</style>
