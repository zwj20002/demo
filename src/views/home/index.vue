<template>
  <div class="container">
    <div class="banner">
      <img src="/src/assets/7f764316716de5182e0791cfd6356e03.png" alt="" />
    </div>
    <div class="sub-content">
      <div class="menus">
        <div class="menu-item">
          <div class="icon">
            <img src="/src/assets/nav_1.png" alt="" />
          </div>
          <div class="font">我的机具</div>
        </div>
        <div class="menu-item">
          <div class="icon">
            <img src="/src/assets/nav_2.png" alt="" />
          </div>
          <div class="font">交易记录</div>
        </div>
        <div class="menu-item">
          <div class="icon">
            <img src="/src/assets/nav_3.png" alt="" />
          </div>
          <div class="font">奖励钱包</div>
        </div>
        <div class="menu-item">
          <div class="icon">
            <img src="/src/assets/nav_4.png" alt="" />
          </div>
          <div class="font">积分钱包</div>
        </div>
      </div>
      <div class="notice">
        <van-notice-bar
          left-icon="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAFQAAABRCAMAAAB7eHFAAAAAAXNSR0IArs4c6QAAAE5QTFRFAAAA/4AA/4cA/4UA/4MA/4YA/4UD/4UC/4QC/4UC/4UC/4QC/4UC/4UC/4QC/4UD/4QD/4QD/4UD/4UC/4QC/4UC/4QC/4QC/4UC/4UDZEqp3AAAABl0Uk5TABAgMEBQYG9wf4CPkJ+gr7C/wM/Q3+Dv8BR0ZuAAAAH2SURBVFjD7ZjZcsMgDEUtTHDiNo4xXqr//9E+tGERwsZLZ/rAfcqAOSOki+xQVUSiYtUYRNPwc4klTh+omFEwiIiIBphJhY9VJLwQOeovE9FwTMQnrDB/FkfUO1rdOWZiC8EmI6pxUMMy01RwawkVPfHMJFW7lTPkQWF2E0+O+enmB8iNFAY38xkzb262pT70odSUnZu6UWa9JBIqGoOBTCMS1EUkCxwwpUZGWvJUk3Kiv3fxxISegqUGLga7+d4bfeCK/KNpq7X4FX69R0c3ChpXpb1Hx/dg52XOPllzlUto8R62gy7bfZzQbWZAbaNQrQ/nXcyAOlMfd1HseUyfKkmoYE8n15bWZWIHQNhpZJShbbVRqCroTkNcywzVNNQ+KJNieuCOBCh///cwGb5rs/ROGvjB9dRheh9UU7f3VVVNpBsK3KmadOTJY0DcdfPU0WiE5dvTNO2FTvRU3awnu6O7j09m6/2iL91sKXJmOutZeTSlrrFLe4oMgQ77oUMEpcU/ADXU/tH7Hw9o6/u0QAu0QAu0QAu0QP8lVB2Bqj9gblAPMleph5kr1BPMJPUUM0E9yWSpp5kcFS9QgYaSF6gqypQmugT6FZZ4vgTa8XcG5yT5i5iTGri/zGflX7yPcFX93aXrABfaSo2IiKO62q5SZkf5DbeAZbtR7jplAAAAAElFTkSuQmCC"
          :scrollable="false"
          background="#FFF6ED"
          color="#5F3333"
        >
          <van-swipe
            vertical
            class="notice-swipe"
            :autoplay="3000"
            :touchable="false"
            :show-indicators="false"
          >
            <van-swipe-item>通告1</van-swipe-item>
            <van-swipe-item>通告2</van-swipe-item>
          </van-swipe>
        </van-notice-bar>
      </div>
      <div class="money">
        <div class="top">
          <div class="lf">
            <div class="avatar">
              <img src="/src/assets/logo.png" alt="" />
            </div>
            <div class="resiger">注册时间：2025-04-07</div>
          </div>
          <div class="rg" @click="showBottom = true">
            <div class="level">前往升级</div>
          </div>
        </div>
        <div class="bottom">
          <div class="jiangli">
            <div class="font">奖励钱包</div>
            <div class="number">0.00</div>
          </div>
          <div class="jiangli">
            <div class="font">奖励钱包</div>
            <div class="number">0.00</div>
          </div>
        </div>
      </div>
      <div class="sales">
        <div class="lf">
          <div class="time">注册时间：2025-04-07</div>
          <div class="guanfang">官方售后受理</div>
          <div class="sub_title">服务问题/交易问题，2小时内急速受理</div>
        </div>
        <div class="rg">
          <div class="shenqing">申请售后</div>
        </div>
      </div>
    </div>

    <!-- popup弹窗 -->
    <div class="pay-popup">
      <van-popup v-model:show="showBottom" round position="bottom" closeable>
        <div class="content">
          <div class="title">特权等级</div>
          <div class="vip-list">
            <div
              class="list-item"
              @click="active = index"
              :class="{ active: active === index }"
              v-for="(item, index) in ['普通会员', '高级会员', '特级会员']"
              :key="index"
            >
              {{ item }}
            </div>
          </div>
          <div class="footer" @click="showPay = true">确定</div>
        </div>
      </van-popup>
    </div>

    <!-- 支付弹窗 -->
    <div class="zhifu">
      <van-popup v-model:show="showPay" round position="bottom" closeable>
        <div class="content">
          <div class="top">￥498.00</div>
          <div class="pay-list">
            <div class="lf">
              <div class="icon"></div>
              <div class="font">微信支付</div>
            </div>
            <div class="rg"></div>
          </div>
          <div class="footer">立即支付</div>
        </div>
      </van-popup>
    </div>
  </div>
</template>

<script setup lang="ts">
import { ref } from "vue";
const showBottom = ref(false);
const showPay = ref(false);
const active = ref(0);
</script>

<style lang="less" scoped>
.container {
  padding-bottom: 30px;
  .banner {
    position: relative;
    z-index: -1;
    img {
      width: 100%;
      height: 250px;
      object-fit: cover;
    }
  }
  .sub-content {
    padding: 0 20px;
    margin-top: -25px;
    .menus {
      padding: 15px;
      box-sizing: border-box;
      display: flex;
      justify-content: space-between;
      background-color: #fff;
      width: 100%;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
      border-radius: 10px;
      .menu-item {
        display: flex;
        flex-direction: column;
        align-items: center;
        .icon {
          img {
            width: 45px;
            height: 45px;
          }
        }
        .font {
          font-weight: 700;
          font-size: 14px;
        }
      }
    }
    .notice {
      margin-top: 20px;
    }
    .money {
      margin-top: 20px;
      width: 100%;
      background: url("/src/assets/5.png") no-repeat center;
      background-size: cover;
      border: 1px solid #f9d6a8;
      border-radius: 10px;
      .top {
        display: flex;
        justify-content: space-between;
        align-items: center;
        border-bottom: 1px solid #f9d6a8;
        padding: 15px;
        .lf {
          display: flex;
          align-items: center;
          .avatar {
            width: 50px;
            height: 50px;
            border-radius: 50%;
            overflow: hidden;
            img {
              width: 100%;
              height: 100%;
            }
          }
          .resiger {
            margin-left: 10px;
            font-size: 14px;
            color: #777777;
          }
        }
        .rg {
          .level {
            background-color: #ff8503;
            padding: 5px 10px;
            color: #fff;
            border-radius: 15px;
            font-weight: 700;
            font-size: 14px;
          }
        }
      }
      .bottom {
        display: flex;
        justify-content: space-between;
        padding: 15px;
        .jiangli {
          display: flex;
          flex-direction: column;
          align-items: center;
          .font {
            color: #333333;
          }
          .number {
            font-size: 20px;
            font-weight: 700;
            margin-top: 10px;
            color: #333333;
          }
        }
      }
    }
    .sales {
      margin-top: 20px;
      width: 100%;
      background-color: #fffbf6;
      border: 1px solid #f9d6a8;
      border-radius: 10px;
      padding: 15px;
      display: flex;
      justify-content: space-between;
      box-sizing: border-box;
      .lf {
        display: flex;
        flex-direction: column;
        justify-content: center;
        .time {
          font-size: 14px;
          color: #666;
        }
        .guanfang {
          font-size: 16px;
          font-weight: 700;
          color: #333333;
          margin: 8px 0;
        }
        .sub_title {
          font-size: 12px;
          color: #777777;
        }
      }
      .rg {
        display: flex;
        align-items: flex-end;
        .shenqing {
          background-color: #ff8503;
          padding: 5px 10px;
          color: #fff;
          border-radius: 15px;
          font-weight: 700;
          font-size: 14px;
        }
      }
    }
  }
}
.notice-swipe {
  height: 40px;
  line-height: 40px;
}
.pay-popup {
  .content {
    padding: 20px;
    .title {
      font-size: 18px;
      font-weight: 700;
      text-align: center;
      margin-bottom: 20px;
    }
    .vip-list {
      .list-item {
        padding: 15px 0;
        text-align: center;
        border-radius: 20px;
        background-color: #f8f8f8;
        font-size: 14px;
        margin: 25px;
      }
      .active {
        background-color: #fff0df;
        color: #ff8503;
        border: 1px solid #ff8503;
      }
    }
    .footer {
      margin-top: 30px;
      height: 45px;
      display: flex;
      justify-content: center;
      align-items: center;
      background-color: #ff8503;
      color: #fff;
      border-radius: 20px;
      font-size: 16px;
    }
  }
}
.zhifu {
  .content {
    padding: 50px 20px 30px;
    .top {
      text-align: center;
      background-color: #f5f5f5;
      padding: 30px 0;
      color: #e11717;
      font-size: 18px;
      font-weight: 700;
      border-radius: 10px;
    }
    .pay-list {
      display: flex;
      justify-content: space-between;
      align-items: center;
      border-bottom: 1px solid #f7f7f7;
      padding: 20px 0;
      margin-top: 15px;
      .lf {
        display: flex;
        align-items: center;
        .icon {
          width: 15px;
          height: 15px;
          background: url("/src/assets/下载\ \(1\).png") no-repeat center;
          background-size: 100% 100%;
        }
        .font {
          font-size: 14px;
          font-weight: 700;
          margin-left: 5px;
        }
      }
      .rg {
        background: url("/src/assets/下载\ \(2\).png") no-repeat center;
        background-size: 100% 100%;
        width: 15px;
        height: 15.5px;
      }
    }
    .footer {
      margin-top: 50px;
      height: 40px;
      display: flex;
      justify-content: center;
      align-items: center;
      background-color: #ff8503;
      color: #fff;
      border-radius: 20px;
      font-size: 16px;
    }
  }
}
::v-deep(.van-notice-bar) {
  border: 1px solid #f9d6a8;
  border-radius: 7px;
}
</style>
