<template>
  <div class="register-page">
    <div class="container">
      <div class="register-form">
        <div class="register-title">注 册</div>
        <div class="register-input-parts">
          <el-input
            class="register-input"
            placeholder="请输入邮箱..."
            prefix-icon="el-icon-date"
            v-model="input1"
          ></el-input>
          <el-input
            class="register-input"
            placeholder="请输入密码..."
            prefix-icon="el-icon-search"
            v-model="input2"
          ></el-input>
          <el-input
            class="register-input"
            placeholder="请确认密码..."
            prefix-icon="el-icon-search"
            v-model="input3"
          ></el-input>
          <el-button>注 册</el-button>
        </div>
      </div>
      <div class="register-signup">
        已有账号?
        <a href="#">登 陆</a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      input1: "",
      input2: "",
      input3: ""
    };
  }
};
</script>

<style lang="less" scoped>
@import "./index.less";
</style>