<template>
  <section class="section">
    <posts></posts>
  </section>
</template>

<script>
import posts from "@/components/posts.vue"
export default {
  name: "Home",
  components:{
    posts
  }
}
</script>

<style scoped>
section{
  background-color: #f49f1c;
  margin: auto;
  display: flex;
  width: 50%;
  align-content: center;
  flex-direction: column;
  border-right: solid whitesmoke;
  border-left: solid whitesmoke;
}
#resetButton{
  float:right;
  margin-right: 5%;
}

</style>