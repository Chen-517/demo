<template>
<div id="GuideChart">
  <a-carousel autoplay>
    <div><img src="https://img1.baidu.com/it/u=2763268316,2865343497&fm=26&fmt=auto&gp=0.jpg" alt=""></div>
    <div><img src="https://img2.baidu.com/it/u=2175702181,3942982460&fm=26&fmt=auto&gp=0.jpg" alt=""></div>
    <div><img src="https://img2.baidu.com/it/u=2850830478,448407215&fm=26&fmt=auto&gp=0.jpg" alt=""></div>
    <div><img src="https://img0.baidu.com/it/u=1247554568,3944534657&fm=26&fmt=auto&gp=0.jpg" alt=""></div>
  </a-carousel>
</div>
</template>

<script>
export default {
  name: "GuideChart"
}
</script>

<style scoped lang="scss">

#GuideChart{
  width: 100%;
  img{
    width: 100%;
    height: 300px;
  }
}
</style>
