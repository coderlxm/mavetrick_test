<template>
  <div class="Header-Container">
    <div class="search"></div>
    <div class="navbar">
      <div>HOME</div>
      <div>ABOUT</div>
      <div>ITEM</div>
      <div>CATEGORY</div>
      <div>NEWS</div>
    </div>
    <div class="rightbox">
      <div class="login" @click="goToLogin">
        LOGIN
        <div class="loginHoverBox">
          <span class="login-item">Login</span>
          <span class="login-item">Sign up</span>
        </div>
      </div>
      <div class="cart"></div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {};
  },
  methods: {
    goToLogin() {},
  },
};
</script>

<style lang="less" scoped>
.Header-Container {
  width: 100%;
  // background-color: deeppink;
  height: 92px;
  position: fixed;
  top: 0;
  background-color: rgba(255, 255, 255, 0.7);
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 0 20px;
  box-sizing: border-box;
  .search {
    width: 50px;
    height: 50px;
    background-color: #161616;
    border-radius: 5px;
  }
  .navbar {
    width: 60%;
    height: 30px;
    display: flex;
    // padding: 0 30px;
    div {
      margin-right: 20px;
    }
  }
  .rightbox {
    display: flex;
    .login {
      width: 90px;
      height: 52px;
      background-color: #161616;
      cursor: pointer;
      line-height: 52px;
      text-align: center;
      color: #fff;
      border-radius: 5px;
      margin-right: 10px;
      position: relative;
      .loginHoverBox {
        display: none;
        width: 140px;
        height: 100px;
        position: absolute;
        right: 0;
        top: 62px;
        box-shadow: 2px 2px 5px #afafaf;
        color: #161616;
      }
    }
    .login:hover {
      // opacity: 75%;
      .loginHoverBox {
        display: flex;
        box-sizing: border-box;
        padding: 0 5px;
        flex-direction: column;
        justify-content: center;
        background-color: rgb(255, 255, 255);
      }
    }
    .cart {
      width: 50px;
      height: 51px;
      background-color: #161616;
      border-radius: 5px;
    }
  }
}
</style>