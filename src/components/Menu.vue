<template>
  <div>
    <div class="menu">
      <img :src="img[0]" height="55px" />

      <el-menu
        :default-active="activeIndex"
        class="el-menu-demo"
        mode="horizontal"
        @select="handleSelect"
      >
        <el-menu-item index="1">首頁</el-menu-item>
        <el-menu-item index="1">理念</el-menu-item>
        <el-menu-item index="1">團隊</el-menu-item>
        <el-menu-item index="1">最新消息</el-menu-item>
        <el-menu-item index="1">回顧</el-menu-item>
        <el-menu-item index="1">更多..</el-menu-item>
      </el-menu>
    </div>
    <el-menu v-if="false" :span="12">
      <el-menu
        default-active="2"
        class="el-menu-vertical-demo"
        @open="handleOpen"
        @close="handleClose"
      >
        <el-menu-item index="1">
          <span slot="title">首頁</span>
        </el-menu-item>
        <el-menu-item index="2">
          <span slot="title">理念</span>
        </el-menu-item>
        <el-menu-item index="3">
          <span slot="title">團隊</span>
        </el-menu-item>
        <el-menu-item index="4">
          <span slot="title">最新消息</span>
        </el-menu-item>
        <el-menu-item index="5">
          <span slot="title">回顧</span>
        </el-menu-item>
        <el-menu-item index="6">
          <span slot="title">更多..</span>
        </el-menu-item>
      </el-menu>
    </el-menu>
  </div>
</template>
<script>
export default {
  data() {
    return {
      img: [require("@/assets/Image/Menu/Logo.png")]
    };
  }
};
</script>
<style lang="scss">
.menu {
  display: flex;
  justify-content: space-between;
}
</style>
