<template>
  <div>
    <button v-on:click="count = 0">Reset likes</button>
  </div>
</template>

<script>
export default {
  name: "likeReset",
  data: function () {
    return {
      counter: 0,
    };
  },
};
</script>

<style scoped></style>
