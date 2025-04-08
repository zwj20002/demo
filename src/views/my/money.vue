<template>
  <div class="money">
    <div class="type">
      <div class="font">提现类型</div>
      <div class="sub">奖励金钱包</div>
    </div>
    <div class="account">
      <div class="one">
        <span>账户金额：</span
        ><span style="color: #ff8503; font-weight: 700">0.00</span>
      </div>
      <div class="num-box">
        <div
          v-for="(num, index) in [20, 50]"
          :key="index"
          class="num"
          :class="{ 'num-active': selectedNum === num }"
          @click="selectNum(num)"
        >
          {{ num }}
        </div>
      </div>
      <div class="num-box">
        <div
          v-for="(num, index) in [100, 200]"
          :key="index"
          class="num"
          :class="{ 'num-active': selectedNum === num }"
          @click="selectNum(num)"
        >
          {{ num }}
        </div>
      </div>
      <div class="man">本次申请满<span style="color:#ff8503;margin: 0 5px;">20</span>元即可提现</div>
    </div>
    <div class="form">
      <div class="form-detail">
        <van-field
          v-model="value"
          label="银行卡号"
          placeholder="请输入银行卡号"
        />
      </div>
      <div class="form-detail">
        <van-field
          v-model="account"
          label="开户行"
          placeholder="请输入开户行"
        />
      </div>
      <div class="form-detail">
        <van-field v-model="username" label="姓名" placeholder="请输入姓名" />
      </div>
    </div>
    <div class="width-btn">立即提现</div>
    <div class="history">提现记录</div>
  </div>
</template>

<script setup lang="ts">
import { ref } from "vue";
const value = ref("");
const account = ref("");
const username = ref("");
const selectedNum = ref<number | null>(null);

const selectNum = (num: number) => {
  selectedNum.value = num;
};
</script>

<style lang="less" scoped>
.money {
  width: 100%;
  height: 100vh;
  box-sizing: border-box;
  overflow: hidden;
  background-color: #f9f9f9;
  padding: 30px 20px;
  .type {
    display: flex;
    justify-content: space-between;
    background-color: #fff;
    padding: 10px 15px;
    border-radius: 10px;
    .font {
      font-weight: 700;
    }
    .sub {
      font-size: 14px;
      color: #222;
    }
  }
  .account {
    background-color: #fff;
    margin-top: 20px;
    padding: 25px 15px;
    border-radius: 15px;
    .one {
    }
    .num-box {
      display: flex;
      .num {
        width: 100px;
        height: 50px;
        display: flex;
        justify-content: center;
        align-items: center;
        background-color: #f8f8f8;
        border-radius: 10px;
        font-weight: 700;
        margin-right: 20px;
        margin-top: 20px;
        cursor: pointer;
      }
      .num-active {
        background-color: #ff8503;
        color: #fff;
      }
    }
  }
  .form {
    .form-detail {
      margin-top: 10px;
    }
  }
  .width-btn {
    width: 100%;
    height: 40px;
    background-color: #ff8503;
    color: #fff;
    display: flex;
    justify-content: center;
    align-items: center;
    border-radius: 10px;
    margin-top: 50px;
    font-weight: 700;
    border-radius: 20px;
  }
  .history {
    margin-top: 20px;
    font-size: 14px;
    color: #222;
    text-align: center;
  }
}
</style>
