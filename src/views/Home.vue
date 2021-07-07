<template>
  <div id="Home">
    <!--  顶部导航栏  -->
    <div class="top">
      <TopNavigation></TopNavigation>
    </div>

    <!--  导播图  -->
    <div class="GuideChart">
      <GuideChart></GuideChart>
    </div>


    <!--  选项  -->
    <div class="option">
      <Option></Option>
    </div>


    <!--  热推  -->
    <div class="recommend">
      <Recommend></Recommend>
    </div>
  </div>
</template>

<script>

import TopNavigation from "../components/Home/TopNavigation";
import GuideChart from "../components/Home/GuideChart";
import Option from "../components/Home/Option";
import Recommend from "../components/Home/Recommend";

export default {
  name: 'Home',
  components: {TopNavigation, GuideChart, Option,Recommend}
}
</script>

<style lang="scss" scoped>
#Home {
  width: 100%;
  height: 100%;
}

</style>
