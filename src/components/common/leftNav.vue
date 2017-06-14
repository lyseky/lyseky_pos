<template>
  <div class="left-nav">
    <div id="logo" class="logo">
      L
    </div>
    <ul>
      <li>
        <i class="icon iconfont icon-taobao"></i>
        <span>收银</span>
      </li>
      <li>
        <i class="icon iconfont icon-taobao"></i>
        <span>店铺</span>
      </li>
      <li>
        <i class="icon iconfont icon-taobao"></i>
        <span>商品</span>
      </li>
      <li>
        <i class="icon iconfont icon-taobao"></i>
        <span>会员</span>
      </li>
      <li>
        <i class="icon iconfont icon-taobao"></i>
        <span>统计</span>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
    name: 'leftNav',
    mounted:function () {
      var logoWidth = document.querySelector('.left-nav').offsetWidth;
      document.getElementById('logo').style.height = logoWidth + 'px';
      document.getElementById('logo').style.lineHeight = logoWidth + 'px';
    },
    data () {
        return {

        }
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
  .logo{
    background: #2c3e50;
    text-align: center;
    font-size: 32px;
    font-weight: bold;
  }
  .left-nav{
    color:#fff;
    font-size:10px;
    height:100%;
    background-color: #1D8ce0;
    float:left;
    width:5%;
  }
  .iconfont{
    font-size:24px;
  }
  .left-nav ul{
    padding:0px;
    margin: 0px;
  }
  .left-nav li{
    list-style: none;
    text-align: center;
    border-bottom:1px solid #20a0ff;
    padding:20px;
  }
  .left-nav li span{
    line-height: 24px;
    height: 24px;
    display: inline-block;
  }
</style>
