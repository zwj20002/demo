<template>
  <div class="my">
    <div class="top-bg"></div>
    <div class="user-info">
      <div class="avatar">
        <img src="/src/assets/logo.png" alt="" />
      </div>
      <div class="info">
        <div class="info-top">
          <div class="nickname">点击填写昵称</div>
          <div class="status">未开通</div>
        </div>
        <div class="register-time">注册时间：2025-04-07</div>
      </div>
    </div>
    <div class="card">
      <div class="one">
        <div class="lf">普通用户</div>
        <div class="center">授权中心</div>
      </div>
      <div class="two">开通特权享受专属福利</div>
      <div class="three">
        <div class="item" @click="goMoney">
          <div class="font">奖励钱包</div>
          <div class="num">0.00</div>
        </div>
        <div class="item" @click="goWithdrawal">
          <div class="font">普通会员<span>待返</span></div>
          <div class="num">0.00</div>
        </div>
        <div class="item">
          <div class="font">积分钱包</div>
          <div class="num">0.00</div>
        </div>
      </div>
    </div>
    <div class="detail">
      <div class="des">
        <div class="icon"><img src="/src/assets/m_1.png" alt="" /></div>
        <div class="font">奖励明细</div>
      </div>
      <div class="des">
        <div class="icon"><img src="/src/assets/m_2.png" alt="" /></div>
        <div class="font">交易记录</div>
      </div>
      <div class="des">
        <div class="icon"><img src="/src/assets/m_3.png" alt="" /></div>
        <div class="font">我的机具</div>
      </div>
      <div class="des">
        <div class="icon"><img src="/src/assets/m_4.png" alt="" /></div>
        <div class="font">积分明细</div>
      </div>
    </div>
    <div class="function">
      <div class="func-item">
        <div class="lf">
          <div class="icon"><img src="/src/assets/l_1.png" alt="" /></div>
          <div class="tile">代理申请</div>
        </div>
        <div class="rg"><img src="/src/assets/下载.png" alt="" /></div>
      </div>
      <div class="func-item">
        <div class="lf">
          <div class="icon"><img src="/src/assets/l_2.png" alt="" /></div>
          <div class="tile">联系客服</div>
        </div>
        <div class="rg"><img src="/src/assets/下载.png" alt="" /></div>
      </div>
      <div class="func-item" @click="goAdvice">
        <div class="lf">
          <div class="icon"><img src="/src/assets/l_3.png" alt="" /></div>
          <div class="tile">意见反馈</div>
        </div>
        <div class="rg"><img src="/src/assets/下载.png" alt="" /></div>
      </div>
      <div class="func-item" @click="goSeting">
        <div class="lf">
          <div class="icon"><img src="/src/assets/l_4.png" alt="" /></div>
          <div class="tile">设置</div>
        </div>
        <div class="rg"><img src="/src/assets/下载.png" alt="" /></div>
      </div>
    </div>
  </div>
</template>
<script setup>
import { useRouter } from "vue-router";
const router = useRouter();
  const goWithdrawal = () => {
    // 跳转到提现页面
    router.push("/withdrawal");
  };
  const goSeting = () => {
    // 跳转到设置页面
    router.push("/seeting");
  };
  const goAdvice = () => {
    // 跳转到意见反馈页面
    router.push("/advice");
  };
  const goMoney = () => {
    // 跳转到奖励钱包页面
    router.push("/money");
  };
</script>
<style scoped lang="less">
.my {
  .top-bg {
    position: absolute;
    z-index: -1;
    width: 100%;
    height: 280px;
    background: url("/src/assets/n_vip.png") no-repeat center center;
  }
  .user-info {
    display: flex;
    align-items: center;
    padding: 0 20px;
    padding-top: 50px;
    .avatar {
      img {
        width: 60px;
        height: 60px;
        border-radius: 50%;
      }
    }
    .info {
      margin-left: 10px;
      .info-top {
        display: flex;
        justify-content: space-between;
        align-items: center;
        .nickname {
          font-weight: 700;
        }
        .status {
          color: #ff8503;
          background-color: #fff;
          padding: 5px 3px;
          border-radius: 10px;
          font-size: 10px;
          margin-left: 10px;
        }
      }
      .register-time {
        font-size: 12px;
        color: #666;
        margin-top: 5px;
      }
    }
  }
  .card {
    background: url("/src/assets/m_bg.png") no-repeat center center;
    background-size: 100% 100%;
    margin: 0 15px;
    border-radius: 10px;
    margin-top: 30px;
    .one {
      display: flex;
      padding: 15px 0 0 15px;
      .lf {
        font-weight: 700;
      }
      .center {
        color: #ee891d;
        background-color: #fff;
        border: 1px solid #ee891d;
        padding: 0 5px;
        border-radius: 10px;
        font-size: 12px;
        margin-left: 10px;
      }
    }
    .two {
      text-align: center;
      color: #ff8503;
      font-weight: 700;
      padding: 15px 0;
      border-bottom: 1px solid #e7e7e7;
    }
    .three {
      display: flex;
      justify-content: space-between;
      padding: 15px;
      .item {
        display: flex;
        flex-direction: column;
        align-items: center;
        .font {
          color: #333333;
          span {
            border-radius: 15px;
            border: 1px solid #ff8503;
            color: #ff8503;
            font-size: 10px;
            padding: 3px 5px;
            margin-left: 5px;
          }
        }
        .num {
          font-size: 20px;
          font-weight: 700;
          margin-top: 10px;
          color: #333333;
        }
      }
    }
  }
  .detail {
    display: flex;
    justify-content: space-between;
    background-color: #fff4ea;
    padding: 15px;
    margin: 0 15px;
    margin-top: 10px;
    border-radius: 10px;
    .des {
      display: flex;
      flex-direction: column;
      align-items: center;
      .icon {
        img {
          width: 35px;
          height: 35px;
        }
      }
      .font {
        font-size: 14px;
        color: #333333;
        margin-top: 5px;
      }
    }
  }
  .function {
    border: 1px solid #f9d6a8;
    padding: 0px 10px;
    margin: 0 15px;
    margin-top: 15px;
    border-radius: 10px;
    .func-item {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 15px 0;
      border-bottom: 1px solid #f4f4f4;
      .lf {
        display: flex;
        align-items: center;
        .icon {
          display: flex;
          flex-direction: column;
          justify-content: center;
          align-items: center;
          margin-right: 10px;
          img {
            width: 25px;
            height: 25px;
          }
        }
        .tile {
        }
      }
      .rg {
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        img {
          width: 20px;
          height: 20px;
        }
      }
    }
  }
}
</style>
