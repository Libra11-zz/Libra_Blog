<template>
  <div class="register-page">
    <div class="container">
      <div class="register-form">
        <div class="register-title">注册</div>
        <div class="register-input-parts">
          <input class="register-input" placeholder="请输入邮箱..." />
          <input class="register-input" placeholder="请输入密码..." />
          <input class="register-input" placeholder="请确认密码..." />
          <input class="register-input button" type="button" value="注册" />
        </div>
      </div>
      <div class="register-signup">
        以有账号?
        <a href="#">登陆</a>
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