<template>
  <div class="seeting">
    <div class="top">
      <div class="item">
        <div class="lf">用户协议</div>
        <div class="rg"><img src="/src/assets/下载.png" alt="" /></div>
      </div>
      <div class="item">
        <div class="lf">隐私政策</div>
        <div class="rg"><img src="/src/assets/下载.png" alt="" /></div>
      </div>
      <div class="item">
        <div class="lf">关于我们</div>
        <div class="rg"><img src="/src/assets/下载.png" alt="" /></div>
      </div>
      <div class="item">
        <div class="lf">清楚缓存</div>
        <div class="rg"><img src="/src/assets/下载.png" alt="" /></div>
      </div>
      <div class="item">
        <div class="lf">注销账号</div>
        <div class="rg"><img src="/src/assets/下载.png" alt="" /></div>
      </div>
    </div>
    <div class="logout">退出登录</div>
  </div>
</template>
<script setup lang="ts"></script>
<style lang="less" scoped>
.seeting {
  padding: 0px 15px;
  padding-top: 10px;
  .top {
    .item {
      display: flex;
      justify-content: space-between;
      padding: 10px 0;
      border-bottom: 1px solid #f7f7f7;
      .lf {
        font-size: 14px;
        color: #333;
      }
      .rg {
        width: 15px;
        height: 15px;
        img {
          width: 100%;
          height: 100%;
        }
      }
    }
  }
  .logout {
    text-align: center;
    color: #fff;
    background-color: #ff8503;
    padding: 12px 0;
    border-radius: 20px;
    margin: 0 auto;
    margin-top: 50px;
  }
}
</style>
