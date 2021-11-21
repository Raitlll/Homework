<template>
  <button v-on:click="count++" id="counter">
    <img src="../assets/like.png" />
  </button>
  <p>{{ count }}</p>
</template>

<script>
export default {
  name: "counter",
  data: function () {
    return {
      count: 0,
    };
  },
};
</script>

<style scoped>
button {
  height: 35px;
  width: 35px;
}
img {
  max-width: 100%;
  max-height: 100%;
}
p {
  font-weight: bolder;
}
</style>
