<template>
  <div class="advice">
    <div class="classfy">
      <div class="title">反馈分类</div>
      <div class="classlist">
        <div
          class="listitem"
          :class="{ active: active === index }"
          @click="active = index"
          v-for="(item, index) in 6"
        >
          分类{{ index + 1 }}
        </div>
      </div>
    </div>
    <div class="question">
      <div class="title">反馈问题</div>
      <div class="textarea">
        <van-field
          v-model="message"
          rows="6"
          autosize
          type="textarea"
          placeholder="请输入反馈的问题"
        />
      </div>
    </div>
    <div class="image">
      <div class="title">问题图片</div>
      <div class="upload"><van-uploader/></div>
    </div>
    <div class="contact">
      <div class="font">联系姓名</div>
      <div class="inputer"><van-field v-model="names" placeholder="请输入姓名" /></div>
    </div>
    <div class="contact">
      <div class="font">联系电话</div>
      <div class="inputer"><van-field v-model="phone" placeholder="请输入电话" /></div>
    </div>
    <div class="submit">提交</div>
  </div>
</template>
<script setup lang="ts">
import { ref } from "vue";
const message = ref("");
const active = ref(0);
const names = ref("");
const phone = ref("");
</script>
<style lang="less" scoped>
.advice {
  padding: 20px;
  .classfy {
    .title {
      font-weight: 700;
    }
    .classlist {
      display: flex;
      justify-content: space-between;
      flex-wrap: wrap;
      font-size: 14px;
      .listitem {
        width: 30%;
        display: flex;
        justify-content: center;
        padding: 10px 0;
        border-radius: 20px;
        background-color: #f5f5f5;
        margin-top: 20px;
      }
      .active {
        background-color: #ff8503;
        color: #fff;
      }
    }
  }
  .question {
    margin-top: 20px;
    .title {
      font-weight: 700;
      margin-top: 20px;
    }
    .textarea {
      margin-top: 20px;
      background-color: #f5f5f5;
    }
  }
  .image {
    .title {
      font-weight: 700;
      margin-top: 20px;
    }
    .upload {
      margin-top: 20px;
    }
  }
  .contact {
    margin-top: 20px;
    .font {
      font-weight: 700;
    }
    .inputer {
      margin-top: 20px;
      background-color: #f5f5f5;
    }
  }
  .submit {
    margin: 30px auto;
    width: 90%;
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
::v-deep(.van-cell) {
  padding: 0;
  background-color: #F5F5F5;
  border-radius: 10px;
}
::v-deep(.van-field__control) {
  padding: 10px 15px;
}
</style>
