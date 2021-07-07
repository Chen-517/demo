<template>
  <div id="Option">
    <ul>
      <li><img alt="" src="//s.qunarzz.com/homenode/images/touchheader/hotel.png">
        <p>酒店</p></li>
      <li><img alt="" src="//s.qunarzz.com/homenode/images/touchheader/flight.png">
        <p>机票</p></li>
      <li><img alt="" src="//s.qunarzz.com/homenode/images/touchheader/train.png">
        <p>火车票</p></li>
      <li><img alt="" src="//s.qunarzz.com/homenode/images/touchheader/piao.png">
        <p>景点门票</p></li>
      <li><img alt="" src="//s.qunarzz.com/homenode/images/touchheader/package.png">
        <p>度假</p></li>
    </ul>

    <ul class="options">
      <li><img alt="" src="https://picbed.qunarzz.com/f5e5770393d759578962e53ee67798c8.png">
        <p>海外酒店</p></li>
      <li><img alt="" src="https://picbed.qunarzz.com/a36d2288f19e54562338f4d8ef986288.png">
        <p>低价机票</p></li>
      <li><img alt="" src="https://picbed.qunarzz.com/377db8cb2143aebf01869c9baad3d325.png">
        <p>汽车票船票</p></li>
      <li><img alt="" src="https://picbed.qunarzz.com/ae617a31e0bd5803d76918b817f6d942.png">
        <p>自由行</p></li>
      <li><img alt="" src="https://picbed.qunarzz.com/1316dc82d1ce6259686d5a68880e5a9d.png">
        <p>攻略</p></li>
    </ul>
    <ul class="options">
      <li><img alt="" src="https://picbed.qunarzz.com/01d2f57f920666364197a850dab859a8.png">
        <p>名宿客栈</p></li>
      <li><img alt="" src="https://picbed.qunarzz.com/83af731055e121a3251690b225327b56.png">
        <p>专车自驾</p></li>
      <li><img alt="" src="https://picbed.qunarzz.com/5b6737be49ca243072ca614f07803b83.png">
        <p>赚钱·信用卡</p></li>
      <li><img alt="" src="https://picbed.qunarzz.com/1e107321f5396ea4994cd832232ecf8a.png">
        <p>旅游团购</p></li>
      <li><img alt="" src="https://picbed.qunarzz.com/c65b3bb7571a6bd62df669213e44b84d.png">
        <p>一日游</p></li>
    </ul>
    <ul class="options">
      <li><img alt="" src="https://picbed.qunarzz.com/f6bb08a239ce1b038204120a8d1e4669.png">
        <p>特惠酒店</p></li>
      <li><img alt="" src="https://picbed.qunarzz.com/3a08f360e958ccb2b947049387873ace.png">
        <p>借钱</p></li>
      <li><img alt="" src="https://picbed.qunarzz.com/19b4f6d2fabd617789fa5aad65b249da.png">
        <p>白金卡</p></li>
      <li><img alt="" src="https://img1.qunarzz.com/order/comp/2007/23/734c3c62d2adce02.png">
        <p>行程设计</p></li>
      <li><img alt="" src="https://picbed.qunarzz.com/25e3b9f17a21a6e0113c57a23ffccde4.png">
        <p>周边短途</p></li>
    </ul>


  </div>
</template>

<script>
export default {
  name: "Option"
}
</script>

<style lang="scss" scoped>

#Option {
  margin-top: 5px;
  width: 100%;
  text-align: center;
  li{
    cursor: pointer;
  }
  .options li {
    width: 80px;
    img {
      width: 50px;
    }

    p{
      font-weight: bold;
    }

  }

  ul {
    display: flex;
    justify-content: space-around;

  }


}


</style>
