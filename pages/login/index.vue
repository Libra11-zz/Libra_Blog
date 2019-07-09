<template>
  <div class="login-page">
    <div class="login-page-container">
      <div class="container">
      <div class="login-form-container">
        <div class="login-form">
        <div class="login-title">登 录</div>
        <div class="login-input-parts">
          <el-input
            class="login-input"
            placeholder="请输入邮箱..."
            prefix-icon="el-icon-user"
            v-model="input1"
          ></el-input>
          <el-input
            class="login-input"
            placeholder="请输入密码..."
            prefix-icon="el-icon-lock"
            v-model="input2"
          ></el-input>
          <el-button>登 录</el-button>
        </div>
      </div>
      </div>
      <div class="login-signup">
        没有账号?
        <a href="#">注 册</a>
      </div>
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