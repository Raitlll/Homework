<template>
  <div v-for="post in getPosts" :key="post.id">
    <div class="postBox">
      <div class="postHeader">
        <img src="../assets/userpic.png" />
        <p>{{ post.date }}</p>
      </div>
      <div class="postDesc">
        <div v-if="post.image">
          <img src="{{post.image}}" />
        </div>
        <div>
          <p>{{ post.description }}</p>
        </div>
        <div class="like">
          <counter></counter>
        </div>
      </div>
    </div>
  </div>
  <like-reset></like-reset>
</template>

<script>
import { mapState } from "vuex";
import Counter from "@/components/counter";
import LikeReset from "@/components/likeReset";
export default {
  name: "posts",
  components: { LikeReset, Counter },
  computed: mapState({
    getPosts: (state) => state.post,
  }),
};
</script>

<style scoped>
.postBox {
  width: 80%;
  background-color: wheat;
  margin: auto;
  margin-top: 20px;
  border-radius: 5px;
  border: 3px solid #2c3e50;
  margin-bottom: 10px;
}
.postHeader {
  border-top-radius: 5px;
  height: 40px;
  width: 100%;
  border-bottom: solid #2c3e50;
}
img {
  max-width: 100%;
  max-height: 100%;
  margin-left: auto;
  margin-right: auto;
  object-fit: fill;
}
.postHeader img {
  margin-left: 20px;
  max-height: 80%;
  max-width: 80%;
  align-content: center;
  border-radius: 50%;
  margin-top: 5px;
  float: left;
}
.postHeader p {
  margin-right: 20px;
  float: right;
}
.postDesc p {
  font-weight: bold;
  font-size: large;
}

</style>
