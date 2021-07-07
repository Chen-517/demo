<template>
  <!-- 热推 -->
  <div id="Recommend">
    <h3>特惠度假</h3>
    <!--  选项卡  -->
    <div :class="{click:quarter}" class="quarter" @click="quarter = true;today=false">当季热门度假</div>
    <div :class="{click:today}" class="today" @click="quarter = false;today=true">今日特惠度假</div>

    <!--  季度热推  -->
    <div v-if="quarter" class="content">
      <ul>
        <li class="fast"><img :src="quarterImages[0]"
                              alt="">
          <p>含往返飞机票(含税)+5晚住宿</p>
          <p class="money">¥ 4500</p>
          <!--     简介     -->
          <div class="introduction">
            <p>北京-泰国</p>
            <p class="title">7天跟团游</p>
          </div>
        </li>
        <li><img :src="quarterImages[0]" alt="">
          <p>含往返飞机票(含税)+5晚住宿</p>
          <p class="money">¥ 4500</p>
          <!--     简介     -->
          <div class="introduction">
            <p>北京-泰国</p>
            <p class="title">7天跟团游</p>
          </div>
        </li>
        <li class="fast"><img :src="quarterImages[0]"
                              alt="">
          <p>含往返飞机票(含税)+5晚住宿</p>
          <p class="money">¥ 4500</p>
          <!--     简介     -->
          <div class="introduction">
            <p>北京-泰国</p>
            <p class="title">7天跟团游</p>
          </div>
        </li>
        <li><img :src="quarterImages[0]" alt="">
          <p>含往返飞机票(含税)+5晚住宿</p>
          <p class="money">¥ 4500</p>
          <!--     简介     -->
          <div class="introduction">
            <p>北京-泰国</p>
            <p class="title">7天跟团游</p>
          </div>
        </li>
      </ul>
      <!--   跳转的详细   -->
      <button>更多特惠度假 ></button>
    </div>
    <!--  今日热推  -->
    <div v-else class="content">
      <ul>
        <li class="fast"><img :src="todayImages[0]"
                              alt="">
          <p>含往返飞机票(含税)+5晚住宿</p>
          <p class="money">¥ 5500</p>
          <!--     简介     -->
          <div class="introduction">
            <p>北京-泰国</p>
            <p class="title">5天跟团游</p>
          </div>
        </li>
        <li><img :src="todayImages[0]" alt="">
          <p>含往返飞机票(含税)+5晚住宿</p>
          <p class="money">¥ 5500</p>
          <!--     简介     -->
          <div class="introduction">
            <p>北京-泰国</p>
            <p class="title">5天跟团游</p>
          </div>
        </li>
        <li class="fast"><img :src="todayImages[0]"
                              alt="">
          <p>含往返飞机票(含税)+5晚住宿</p>
          <p class="money">¥ 5500</p>
          <!--     简介     -->
          <div class="introduction">
            <p>北京-泰国</p>
            <p class="title">5天跟团游</p>
          </div>
        </li>
        <li><img :src="todayImages[0]" alt="">
          <p>含往返飞机票(含税)+5晚住宿</p>
          <p class="money">¥ 5500</p>
          <!--     简介     -->
          <div class="introduction">
            <p>北京-泰国</p>
            <p class="title">5天跟团游</p>
          </div>
        </li>
      </ul>
    </div>
    <!--   跳转的详细   -->
    <button>更多特惠度假 ></button>
  </div>
</template>

<script>
export default {
  name: "Recommend",
  data() {
    return {
      quarter: true,
      today: false,
      //  季度热推图片
      quarterImages: ['//imgs.qunarzz.com/p/p48/201302/28/bc44faa497db0dcf93835fbb.jpg_256x160_0ba13461.jpg'],
      //  今日热推图片
      todayImages: ['//imgs.qunarzz.com/vs_ceph_b2c_001/ffeb9f29-e7e7-4626-8087-ad48c57c4f76.jpg_r_480x320x95_63377b6c.jpg']
    }
  }
}
</script>

<style lang="scss" scoped>
#Recommend {
  h3 {
    font-size: 23px;
    font-weight: bold;
    text-indent: 10px;
  }

  .quarter, .today {
    display: inline-block;
    width: 150px;
    margin-left: 20px;
    text-align: center;
    height: 40px;
    border-radius: 5px;
    line-height: 40px;
    box-shadow: 0 0 3px rgb(85, 85, 85);
    transition: all .3s;
    cursor: pointer;
    font-size: 18px;
  }

  .click {
    background: #17C0C8;
    color: #ffff;
  }

  .content {
    position: relative;
    width: 100%;
    padding: 10px;

    ul li {
      position: relative;
      display: inline-block;
      width: 280px;

      &.fast {
        margin-right: 10px;
      }

      .introduction {
        text-align: center;
        position: absolute;
        width: 150px;
        top: 124px;
        left: 0;
        right: 0;
        margin: auto;
        background: rgba(0, 0, 0, 0.6);
        color: #ffff;

        .title {
          font-size: 14px;
          color: #ffde00;
        }
      }

      img {
        width: 100%;
        border-radius: 10px;
      }

      p {
        text-indent: 10px;
        margin-bottom: 0;
        font-size: 20px;
        overflow: hidden;
        text-overflow: ellipsis;
        white-space: nowrap;

        &.money {
          color: #ff7400;
          font-size: 25px;
          font-weight: bold;
        }
      }
    }


    button {
      border: 0 none;
      background: none;
      border-radius: 5px;
      outline: none;

    }


  }


}
</style>
