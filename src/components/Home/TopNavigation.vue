<template>
  <div id="TopNavigation">
    <div class="left">
      <a-icon type="left"/>
    </div>
    <div class="input "><span class="iconfont">&#xe65c;</span>
      <input maxlength="30" placeholder="输入城市/景点/游玩主题" type="text">
    </div>
    <div class="right">
      <a-dropdown :trigger="['click']" class="col">
        <a class="ant-dropdown-link" @click="e => e.preventDefault()">
          城市
          <a-icon style="font-size: 20px" type="down"/>
        </a>
        <a-menu slot="overlay">

          <a-sub-menu key="index" title="安徽省">
            <a-menu-item>合肥市</a-menu-item>
            <a-menu-item>芜湖市</a-menu-item>
          </a-sub-menu>

          <a-sub-menu key="test" title="浙江省">
            <a-menu-item>杭州市</a-menu-item>
            <a-menu-item>温州市</a-menu-item>
          </a-sub-menu>

        </a-menu>
      </a-dropdown>
    </div>
  </div>
</template>

<script>
export default {
  name: "TopNavigation",
  data() {
    return {}
  }
}
</script>

<style lang="scss" scoped>
@font-face {
  font-family: 'iconfont';  /* Project id 2655200 */
  src: url('//at.alicdn.com/t/font_2655200_u2hrb81k6wp.woff2?t=1625557721443') format('woff2'),
  url('//at.alicdn.com/t/font_2655200_u2hrb81k6wp.woff?t=1625557721443') format('woff'),
  url('//at.alicdn.com/t/font_2655200_u2hrb81k6wp.ttf?t=1625557721443') format('truetype');
}

.iconfont {
  font-family: "iconfont" !important;
  font-size: 16px;
  font-style: normal;
  -webkit-font-smoothing: antialiased;
  -webkit-text-stroke-width: 0.2px;
  -moz-osx-font-smoothing: grayscale;
}


#TopNavigation {
  box-sizing: border-box;
  position: relative;
  height: 65px;
  width: 100%;
  background: #01B3CD;
  padding: 10px 0;
  color: #ffff;

  .left {
    position: relative;
    float: left;
    height: 100%;
    font-size: 30px;
    top: 2px;
    left: 5px;
  }

  input::-webkit-input-placeholder {
    color: #acacac;
  }

  input::-ms-input-placeholder {
    color: #acacac;
  }

  .input {
    position: absolute;
    left: 50px;
    height: 45px;
    font-size: 20px;
    color: #acacac;
    background: #ffff;
    width: 450px;
    line-height: 45px;
    box-sizing: border-box;
    padding: 0 10px;
    text-align: left;
    border-radius: 5px;

    input {
      height: 45px;
      width: 90%;
      background: none;
      border: none;
      outline: none;
      color: black;
    }

    .iconfont {
      margin-right: 10px;
      cursor: pointer;
    }
  }


  .right {
    margin-right: 10px;
    float: right;
    font-size: 20px;
    line-height: 45px;
    height: 45px;
    width: 70px;
  }

  .col {
    color: #ffff;
  }

}
</style>
