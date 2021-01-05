<template>
  <div id="title">
    <div class="left">
      <img id="welcome_logo" src="../assets/logo.jpg" alt="logo">
    </div>
    <div class="middle">

    </div>
    <div class="right">
      <h1>{{ msg }}</h1>
      <div class="right-bottom">
        <el-button id="toIndex_button" @click="btnClick1" round type="primary">
          <svg class="icon" aria-hidden="true">
            <use xlink:href="#icon-jinru"></use>
          </svg> Platfrom1
        </el-button>
        <el-button id="toIndex_button" @click="btnClick2" round type="primary">
          <svg class="icon" aria-hidden="true">
            <use xlink:href="#icon-jinru"></use>
          </svg> Platfrom2
        </el-button>
        <el-button id="toIndex_button" @click="btnClick3" round type="primary">
          <svg class="icon" aria-hidden="true">
            <use xlink:href="#icon-jinru"></use>
          </svg> Platfrom3
        </el-button>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: "Welcome",
    data() {
      return {
        msg: '可视化数据分析平台',
      }
    },
    methods: {
      btnClick1() {
        this.$router.push('/index/projectView');
      },
      btnClick2() { // platfrom2 push

      },
      btnClick3() { // platform3 push

      }
    }
  }
</script>

<style scoped>

  #title {
    display: block;
  }

  #title .left #welcome_logo {
    height: 121px;
    width: 118px;
    -webkit-clip-path: circle(50% at 50% 50%);
    clip-path: circle(50% at 50% 50%);
    margin-left: 10px;
    min-height: 51px;
    min-width: 48px;
    -webkit-box-align: end;
    -ms-flex-align: end;
    align-items: flex-end;
  }

  #title .right h1, h2 {
    font-weight: normal;
    font-size: 30px;
    text-align: left;

  }
  #title .right .right-bottom {
    display: block;
    text-align: left;
  }

  #title .left, #title .middle, #title .right {
    display: inline-block;
    vertical-align: baseline;
    margin-left: 10px;
  }

</style>
