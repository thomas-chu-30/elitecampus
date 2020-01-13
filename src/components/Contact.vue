<template>
  <div class="contact">
    <el-row class="row">
      <el-col class="col" :xs="24" :md="12">
        <h2>定閱我們</h2>
        <p>感謝您關注Elite Campus，當有新的賽事與活動，將會寄送邀請給您。</p>
        <p>tw.elitecampus@gmail.com |</p>
      </el-col>
      <el-col class="col" :xs="24" :md="12">
        <h2>我想收到活動消息</h2>
        <el-input v-model="input" placeholder="mail"></el-input>
        <el-button type="warning">訂閱</el-button>
      </el-col>
    </el-row>
  </div>
</template>
<script>
export default {
  data() {
    return {
      input: ""
    };
  }
};
</script>
<style lang="scss">
.contact {
  display: flex;
  align-items: center;
  justify-content: center;
  color: white;
  background-color: #082a63;
  min-height: 360px;
  .row {
    width: 80%;
    // height: 900px;
    display: flex;
    align-items: center;
    .col {
      padding: 30px;
      // display: flex;
      // align-items:center:
    }
  }
}
</style>
