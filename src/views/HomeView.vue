<template>
  <div class="home">
    <Header />
    <div class="column">
      <a href="" class="titleImg">
        <img :src="imgUrl" />
      </a>
      <List />
    </div>
  </div>
</template>

<script>
// @ is an alias to /src

import Header from "@/components/Header";
import List from "@/components/List";
export default {
  name: "HomeView",
  data() {
    return {
      imgUrl: require("@/assets/img/1.jpeg"),
    };
  },
  components: {
    Header,
    List,
  },
};
</script>

<style lang="less" scoped>
.column {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  margin-top: 60px;
  .titleImg {
    width: 80%;
    display: flex;
    margin-top: 90px;
    margin-bottom: 50px;
    img {
      width: 100%;
    }

  }
}
</style>
