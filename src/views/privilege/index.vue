<template>
    <div class="container">
        <div class="bg">
            <div class="vip">
                <div class="title">会员特权</div>
                <div class="read"><span style="color: #fff;">同意</span><span style="color: #FFE3B6;">《特权服务协议》</span>
                </div>
                <div class="enjoy">
                    享用特权
                </div>
                <div class="gift">购买特权礼包既享各种服务权益</div>
            </div>
            <div class="member">特权会员权益</div>
            <div class="merber-list">
                <div class="item">
                    <div class="icon"><img src="/src/assets/p_1.png" alt=""></div>
                    <div class="font">返现</div>
                    <div class="sub-title">获得更多返现</div>
                </div>
                <div class="item">
                    <div class="icon"><img src="/src/assets/p_2.png" alt=""></div>
                    <div class="font">商户</div>
                    <div class="sub-title">专属特权商户</div>
                </div>
                <div class="item">
                    <div class="icon"><img src="/src/assets/p_3.png" alt=""></div>
                    <div class="font">身份</div>
                    <div class="sub-title">会员身份标识</div>
                </div>
                <div class="item">
                    <div class="icon"><img src="/src/assets/p_4.png" alt=""></div>
                    <div class="font">分红</div>
                    <div class="sub-title">每天都可参与</div>
                </div>
                <div class="item">
                    <div class="icon"><img src="/src/assets/p_5.png" alt=""></div>
                    <div class="font">代发</div>
                    <div class="sub-title">企业一键代发</div>
                </div>
                <div class="item">
                    <div class="icon"><img src="/src/assets/p_6.png" alt=""></div>
                    <div class="font">会员工具</div>
                    <div class="sub-title">可赚取高额收益</div>
                </div>
                <div class="item">
                    <div class="icon"><img src="/src/assets/p_7.png" alt=""></div>
                    <div class="font">客服</div>
                    <div class="sub-title">个人专属客服</div>
                </div>
                <div class="item">
                    <div class="icon"><img src="/src/assets/p_8.png" alt=""></div>
                    <div class="font">换机</div>
                    <div class="sub-title">终身免费换机</div>
                </div>

            </div>
            <div class="shouyi">
                <div class="title">会员收益</div>
                <div class="content">
                    <div class="lf">
                        <div class="detail">会员每日分红</div>
                        <div class="desc"><span>*</span>交易越多，分红领取越多，金额上不封顶</div>
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
                <div class="descript">保障说明保障说明保障说明保障说明保障说明保障说明保障说明保障说明</div>
            </div>
        </div>
        特权
    </div>
</template>
<script setup>
</script>
<style scoped lang="less">
.container {
    .bg {
        width: 100%;
        height: 100vh;
        background: url("/src/assets/p_bg.png") no-repeat center center / cover;

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
                border: 3px solid #FFAE75;
                border-radius: 20px;
                background-color: #FF6E47;
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
                background-color: #FFA45B;
                text-align: center;
                padding: 10px 0;
                border-radius: 5px;
                margin-top: 50px;
                font-weight: 700;
            }
        }

        .member {
            color: #FE8A28;
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
                    color: #9A9A9A;
                }
            }
        }
        .shouyi {
            margin-top: 50px;
            background-color: #FFFBF1;
            border-radius: 10px;
            padding: 0px 10px;
            margin: 0 20px;
            margin-top: 30px;
            .title {
                color: #FFA748;
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
                            color: #FF6E47;
                            font-weight: 700;
                            margin-right: 5px;
                        }
                    }
                }
                .rg {
                    border-radius: 20px;
                    background-color: #FF8502;
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
            background-color: #FFFBF1;
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
                    color: #FF6E47;
                    font-weight: 700;
                    margin-right: 5px;
                }
            }
        }


    
}
}


</style>