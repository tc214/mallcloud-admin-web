<template>
  <div class="header">
    <div class="header-in w">
      <div class="header-l">
        <img src="../../../assets/images/logo.png">
        <ul>
          <li><a href="http://www.baidu.com" target="_blank" class="header-font">百度</a></li>
          <li><a href="http://www.github.com/index.html" class="header-font" target="_blank">github</a></li>
          <li><a href="http://www.mallcloud.net" class="header-font" target="_blank">Cloud</a></li>
        </ul>
      </div>
      <div class="header-r">
        <ul>
          <li><a @click="goSignUp" class="header-font">注册</a></li>
          <li><a @click="goSignIn" class="header-font">登录</a></li>
          <!--<li><a @.prevent.click="logout" class="header-font">登录</a></li>-->
          <li><a @click.prevent="logOut" class="header-font">退出</a></li>
        </ul>
      </div>
    </div>
  </div>
</template>
<style rel="stylesheet/scss" lang="scss">
  .header {
    background-color: #303643;
    height: 46px;
    position: absolute;
    z-index: 10;
    width: 100%;
  }
  .header-in {
    width: 1000px;
    height: 46px;
  }
  .header-l, .header-r {
    width: 500px;
    height: 46px;
  }
  .header-l {
    float: left;
  }

  .header-font {
    font-size: 14px;
    cursor:pointer;
  }

  .header-r {
    float: left;
  }
  .header-l img {
    width: 100px;
    height: 30px;
    margin-top: 9px;
    float: left;
  }
  .header-l li {
    float: left;
    height: 46px;
    line-height: 46px;
    margin: 0 18px;

  }

  .header-r input {
    outline: 0;
    float: left;
    width: 203px;
    height: 26px;
    margin-left: 170px;
    margin-top: 10px;
    border: 1px solid #8c92a4;
    border-radius: 50px;
    background-color: #303643;
    text-indent: 1em;
    color: #8c92a4
  }

  .header-r li {
    height: 46px;
    line-height: 46px;
    margin: 0 10px;
    color: #8c92a4;
    float: right;
  }

  .header-r li a {
    color: #8c92a4;
  }
</style>

