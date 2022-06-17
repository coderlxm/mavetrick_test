<template>
  <div class="column2">
    <ul class="list">
      <li v-for="item in listItem" :key="item.id">
        <img src="../assets/img/2.webp" alt="" />
        <span class="itemname">{{ item.name }}</span>
        <span class="itemprice">{{ item.price }}</span>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      listItem: [
        { id: 1, name: "Turning Point", price: "780JPY" },
        { id: 2, name: "Turning Point", price: "780JPY" },
        { id: 3, name: "Turning Point", price: "780JPY" },
        { id: 4, name: "Turning Point", price: "780JPY" },
        { id: 5, name: "Turning Point", price: "780JPY" },
        { id: 6, name: "Turning Point", price: "780JPY" },
        { id: 7, name: "Turning Point", price: "780JPY" },
        { id: 8, name: "Turning Point", price: "780JPY" },
      ],
    };
  },
};
</script>

<style lang="less" scoped>
.column2 {
  width: 80%;
  .list {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    list-style-type: none;
    li {
      width: 185px;
      height: 230px;
      // background-color: #bfa;
      margin-bottom: 30px;
      display: flex;
      flex-direction: column;
      justify-content: space-between;
      .itemprice {
      }
    }
  }
}
</style>