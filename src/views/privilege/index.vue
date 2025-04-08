<template>
  <div class="container">
    <div class="bg">
      <div class="vip">
        <div class="title">会员特权</div>
        <div class="read">
          <span style="color: #fff">同意</span
          ><span style="color: #ffe3b6">《特权服务协议》</span>
        </div>
        <div class="enjoy">享用特权</div>
        <div class="gift">购买特权礼包既享各种服务权益</div>
      </div>
      <div class="member">特权会员权益</div>
      <div class="merber-list">
        <div class="item">
          <div class="icon"><img src="/src/assets/p_1.png" alt="" /></div>
          <div class="font">返现</div>
          <div class="sub-title">获得更多返现</div>
        </div>
        <div class="item">
          <div class="icon"><img src="/src/assets/p_2.png" alt="" /></div>
          <div class="font">商户</div>
          <div class="sub-title">专属特权商户</div>
        </div>
        <div class="item">
          <div class="icon"><img src="/src/assets/p_3.png" alt="" /></div>
          <div class="font">身份</div>
          <div class="sub-title">会员身份标识</div>
        </div>
        <div class="item">
          <div class="icon"><img src="/src/assets/p_4.png" alt="" /></div>
          <div class="font">分红</div>
          <div class="sub-title">每天都可参与</div>
        </div>
        <div class="item">
          <div class="icon"><img src="/src/assets/p_5.png" alt="" /></div>
          <div class="font">代发</div>
          <div class="sub-title">企业一键代发</div>
        </div>
        <div class="item">
          <div class="icon"><img src="/src/assets/p_6.png" alt="" /></div>
          <div class="font">会员工具</div>
          <div class="sub-title">可赚取高额收益</div>
        </div>
        <div class="item">
          <div class="icon"><img src="/src/assets/p_7.png" alt="" /></div>
          <div class="font">客服</div>
          <div class="sub-title">个人专属客服</div>
        </div>
        <div class="item">
          <div class="icon"><img src="/src/assets/p_8.png" alt="" /></div>
          <div class="font">换机</div>
          <div class="sub-title">终身免费换机</div>
        </div>
      </div>
      <div class="shouyi">
        <div class="title">会员收益</div>
        <div class="content">
          <div class="lf">
            <div class="detail">会员每日分红</div>
            <div class="desc">
              <span>*</span>交易越多，分红领取越多，金额上不封顶
            </div>
          </div>
          <div class="rg">前往参与</div>
        </div>
        <div class="content">
          <div class="lf">
            <div class="detail">团队奖励</div>
            <div class="desc"><span>*</span>成员有激活，团队收益自动入账</div>
          </div>
          <div class="rg">查看团队</div>
        </div>
      </div>
      <div class="baozhang">
        <div class="titles">保障说明</div>
        <div class="descript">
          保障说明保障说明保障说明保障说明保障说明保障说明保障说明保障说明
        </div>
      </div>
    </div>
    <!-- <div class="active">
      <div class="active-title">有激活就有会员分红奖励</div>
      <div class="sub-title">邀请激活获刷卡返现</div>
      <div class="table">
        <div class="th">
          <div>特权</div>
          <div>普通用户</div>
          <div>特权会员</div>
        </div>
        <div class="td">
          <div>秒到费</div>
          <div>可领1笔</div>
          <div>无限制</div>
        </div>
      </div>
    </div> -->
    <div class="active">
    <div class="active-title">有激活就有会员分红奖励</div>
    <div class="sub-title">邀请激活获刷卡返现</div>
    <div class="comparison-table">
      <div class="table-header">
        <div class="header-item">特权</div>
        <div class="header-item">普通用户</div>
        <div class="header-item highlight">特权会员</div>
      </div>
      
      <div class="table-row">
        <div class="row-title">秒到费</div>
        <div class="row-value">可领1笔</div>
        <div class="row-value highlight">无限制</div>
      </div>
      
      <div class="table-row">
        <div class="row-title">返现特权</div>
        <div class="row-value">万3</div>
        <div class="row-value highlight">会员商费率</div>
      </div>
      
      <div class="table-row">
        <div class="row-title">会员身份</div>
        <div class="row-value x-mark">X</div>
        <div class="row-value highlight">长期享用</div>
      </div>
      
      <div class="table-row">
        <div class="row-title">会员工具</div>
        <div class="row-value x-mark">X</div>
        <div class="row-value highlight">可赚取高额收益</div>
      </div>
      
      <div class="table-row">
        <div class="row-title">会员分红</div>
        <div class="row-value x-mark">X</div>
        <div class="row-value highlight">长期分润</div>
      </div>
      
      <div class="table-row">
        <div class="row-title">特权商户</div>
        <div class="row-value x-mark">X</div>
        <div class="row-value highlight checkmark">✓</div>
      </div>
      
      <div class="table-row">
        <div class="row-title">专属客服</div>
        <div class="row-value x-mark">X</div>
        <div class="row-value highlight checkmark">✓</div>
      </div>
      
      <div class="table-row">
        <div class="row-title">终身换机</div>
        <div class="row-value x-mark">X</div>
        <div class="row-value highlight checkmark">✓</div>
      </div>
    </div>
  </div>
  </div>
</template>
<script setup></script>
<style scoped lang="less">
.container {
  .bg {
    width: 100%;
    background: url("/src/assets/p_bg.png") no-repeat;
    background-size: 100% 100%;
    .vip {
      margin: 0 30px;

      .title {
        font-size: 36px;
        color: #fff;
        font-weight: 700;
      }

      .read {
        margin-top: 10px;
      }

      .enjoy {
        width: 100px;
        height: 35px;
        border: 3px solid #ffae75;
        border-radius: 20px;
        background-color: #ff6e47;
        color: #fff;
        font-weight: 700;
        display: flex;
        justify-content: center;
        align-items: center;
        font-size: 14px;
        margin-top: 30px;
      }

      .gift {
        margin-top: 10px;
        color: #fff;
        background-color: #ffa45b;
        text-align: center;
        padding: 10px 0;
        border-radius: 5px;
        margin-top: 70px;
        font-weight: 700;
      }
    }

    .member {
      color: #fe8a28;
      text-align: center;
      font-weight: 700;
      margin-top: 20px;
    }

    .merber-list {
      display: flex;
      flex-wrap: wrap;
      justify-content: space-between;

      .item {
        width: 25%;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        margin-top: 15px;

        .icon {
          width: 30px;
          height: 30px;

          img {
            width: 100%;
            height: 100%;
          }
        }

        .font {
          font-size: 14px;
          color: #323232;
          font-weight: 700;
          margin: 5px 0;
        }

        .sub-title {
          font-size: 10px;
          color: #9a9a9a;
        }
      }
    }
    .shouyi {
      margin-top: 50px;
      background-color: #fffbf1;
      border-radius: 10px;
      padding: 0px 10px;
      margin: 0 20px;
      margin-top: 30px;
      .title {
        color: #ffa748;
        padding: 15px 0;
      }
      .content {
        display: flex;
        justify-content: space-between;
        align-items: center;
        margin-bottom: 15px;
        padding-bottom: 15px;
        .lf {
          .detail {
            font-size: 14px;
            color: #323232;
            font-weight: 700;
          }

          .desc {
            font-size: 12px;
            color: #666;
            margin-top: 5px;
            span {
              color: #ff6e47;
              font-weight: 700;
              margin-right: 5px;
            }
          }
        }
        .rg {
          border-radius: 20px;
          background-color: #ff8502;
          color: #fff;
          font-weight: 700;
          display: flex;
          justify-content: center;
          align-items: center;
          font-size: 14px;
          padding: 5px 10px;
        }
      }
    }
    .baozhang {
      margin-top: 20px;
      background-color: #fffbf1;
      border-radius: 10px;
      padding: 0px 10px;
      margin: 0 20px;
      .titles {
        color: #000;
        padding: 15px 0;
        text-align: center;
        font-weight: 700;
      }
      .descript {
        color: #666;
        padding-bottom: 20px;
        span {
          color: #ff6e47;
          font-weight: 700;
          margin-right: 5px;
        }
      }
    }
  }
//   .active {
//     background-color: #ffeeb8;
//     padding-bottom: 80px;
//     padding-top: 20px;
//     .active-title {
//       color: #fff;
//       padding: 10px 0px;
//       border-radius: 10px;
//       font-weight: 700;
//       background-color: #ffb66c;
//       margin: 0 50px;
//       text-align: center;
//       font-size: 14px;
//     }
//     .sub-title {
//       text-align: center;
//       color: #ff8502;
//       font-size: 12px;
//       font-weight: 700;
//       margin: 20px 0;
//     }
//     .table {
//       margin: 0 20px;
//       border: 2px solid #fff;
//       border-radius: 10px;
//       .th {
//         display: flex;
//         justify-content: space-between;
//         font-weight: 700;
//         background-color: #ffeee4;
//         padding: 15px 0;
//         font-size: 14px;
//       }
//       .td {
//         display: flex;
//         justify-content: space-between;
//         padding: 15px 0;
//         background-color: #fffbf6;
//         font-size: 12px;
//       }
//     }
//   }
.active {
  background-color: #FFEEB8;
  padding-bottom: 80px;
  padding-top: 20px;
  
  .active-title {
    color: #fff;
    padding: 10px 0px;
    border-radius: 10px;
    font-weight: 700;
    background-color: #ffb66c;
    margin: 0 50px;
    text-align: center;
    font-size: 14px;
  }
  
  .sub-title {
    text-align: center;
    color: #FF8502;
    font-size: 12px;
    font-weight: 700;
    margin: 20px 0;
  }
  
  .comparison-table {
    width: calc(100% - 40px);
    margin: 0 auto;
    background-color: #FFFAEA;
    border-radius: 10px;
    overflow: hidden;
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
    border: 2px solid #fff;
    .table-header {
      display: flex;
      background-color: #FFEDE2;
      border-bottom: 1px solid #eaeaea;
      .header-item {
        flex: 1;
        text-align: center;
        padding: 15px 10px;
        font-weight: bold;
        color: #333;
        font-size: 14px;
        &:first-child {
          flex: 1.2;
        }
      }
    }
    
    .table-row {
      display: flex;
      border-bottom: 1px solid #eaeaea;
      &:last-child {
        border-bottom: none;
      }
      
      .row-title {
        flex: 1.2;
        padding: 15px 10px;
        font-weight: 500;
        text-align: center;
      }
      
      .row-value {
        flex: 1;
        padding: 15px 10px;
        text-align: center;
        color: #666;
        &.highlight {
        //   color: #ff6e47;
          font-weight: 500;
        }
        
        &.checkmark {
          color: #4CAF50;
          font-weight: bold;
        }
        
        &.x-mark {
          color: #9E9E9E;
        }
      }
    }
  }
}
}
</style>
