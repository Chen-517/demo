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



  </div>
</template>

<script>

import TopNavigation from "../components/TopNavigation";
import GuideChart from "../components/GuideChart";

export default {
  name: 'Home',
  components: {TopNavigation, GuideChart}
}
</script>

<style lang="scss" scoped>
#Home {
  width: 100%;
  height: 100%;
}

</style>
