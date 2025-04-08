<template>
  <!-- <van-nav-bar
    v-if="showNavbar"
    :title="(route.meta.title as string)"
    left-text="返回"
    left-arrow
    @click-left="router.back()"
  /> -->
  <router-view />
  <van-tabbar 
    v-if="showTabbar" 
    v-model="active" 
    active-color="#FF8503" 
    route 
    style="background-color:#F7F7FA;border-top: 1px solid #ccc;"
  > 
    <van-tabbar-item replace to="/home">
      <span>首页</span>
      <template #icon="props">
        <img :src="props.active ? icon[0].active : icon[0].inactive" />
      </template>
    </van-tabbar-item>
    <van-tabbar-item replace to="/privilege">
      <span>特权</span>
      <template #icon="props">
        <img :src="props.active ? icon[1].active : icon[1].inactive" />
      </template>
    </van-tabbar-item>
    <van-tabbar-item replace to="/my">
      <span>我的</span>
      <template #icon="props">
        <img :src="props.active ? icon[2].active : icon[2].inactive" />
      </template>
    </van-tabbar-item>
  </van-tabbar>
</template>

<script setup lang="ts">
import { ref, computed } from "vue";
import { useRoute } from "vue-router";

const route = useRoute();
const active = ref(0);
const icon = [
  {
    active: "http://0806gc.62.hzgqapp.com/static/tarbar/icon_1_s.png",
    inactive: "http://0806gc.62.hzgqapp.com/static/tarbar/icon_1.png",
  },
  {
    active: "http://0806gc.62.hzgqapp.com/static/tarbar/icon_2_s.png",
    inactive: "http://0806gc.62.hzgqapp.com/static/tarbar/icon_2.png",
  },
  {
    active: "http://0806gc.62.hzgqapp.com/static/tarbar/icon_3_s.png",
    inactive: "http://0806gc.62.hzgqapp.com/static/tarbar/icon_3.png",
  },
];

const showTabbar = computed(() => {
  const currentPath = route.path;
  return ['/home', '/privilege', '/my'].includes(currentPath);
});

// import { computed } from 'vue'
// import { useRoute, useRouter } from 'vue-router'

// const route = useRoute()
// const router = useRouter()
// const showNavbar = computed(() => { return route.meta.showNavbar })
</script>

<style lang="less" scoped>
::v-deep(.van-tabbar) {
  background: red;
}
</style>