<template>
  <div class="login-page">
    <div class="container">
      <div class="login-form">
        <div class="login-title">登 陆</div>
        <div class="login-input-parts">
          <input class="login-input" placeholder="请输入邮箱..." />
          <input class="login-input" placeholder="请输入密码..." />
          <input class="login-input button" type="button" value="登 陆" />
        </div>
        <div class="login-forgot">忘记密码？</div>
      </div>
      <div class="login-signup">
        没有账号?
        <a href="#">注 册</a>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="less" scoped>
@import "./index.less";
</style>