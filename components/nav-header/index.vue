<style lang="less">
@import "./index";
</style>
<template>
  <header class="nav-header">
    <div class="left">
      <nuxt-link to="/home" class="logo">
        <i class="iconfont icontianchengzuo"></i>
      </nuxt-link>
      <div class="directory">
        <nuxt-link to="/home" class="home">
          <i class="iconfont iconhome"></i>首页
        </nuxt-link>
        <nuxt-link to="/book" class="book">
          <i class="iconfont iconbooks"></i>书籍
        </nuxt-link>
        <nuxt-link to="/blog" class="blog">
          <i class="iconfont iconblog"></i>博客
        </nuxt-link>
        <nuxt-link to="/lab" class="lab">
          <i class="iconfont iconlab"></i>实验室
        </nuxt-link>
        <nuxt-link to="/contact" class="contact">
          <i class="iconfont iconContact-Info"></i>联系我
        </nuxt-link>
      </div>
    </div>
    <div class="right">
      <div class="mobile-nav">
        <div class="nav-logo">
          <i class="iconfont iconnav" @click="showMobileMenu"></i>
        </div>
      </div>
      <div class="personal">
        <div class="avatar">
          <img src="https://pic.qqtn.com/up/2018-5/15252271245423063.jpg" alt />
          <ul class="personal-info">
            <li>
              <nuxt-link to="/personal">个人中心</nuxt-link>
            </li>
            <li>
              <nuxt-link to="/logout">退 出</nuxt-link>
            </li>
          </ul>
        </div>
      </div>
      <div class="search">
        <input class="search-input" type="text" placeholder="请输入你要搜索的内容" />
        <i class="iconfont iconsearch"></i>
      </div>
    </div>
    <ul class="mobile-menu" ref="mobileMenu">
      <li>
        <nuxt-link to="/home" class="home">
          <i class="iconfont iconhome"></i> 首页
        </nuxt-link>
      </li>
      <li>
        <nuxt-link to="/book" class="book">
          <i class="iconfont iconbooks"></i> 书籍
        </nuxt-link>
      </li>
      <li>
        <nuxt-link to="/blog" class="blog">
          <i class="iconfont iconblog"></i> 博客
        </nuxt-link>
      </li>
      <li>
        <nuxt-link to="/lab" class="lab">
          <i class="iconfont iconlab"></i> 实验室
        </nuxt-link>
      </li>
      <li>
        <nuxt-link to="/contact" class="contact">
          <i class="iconfont iconContact-Info"></i> 联系我
        </nuxt-link>
      </li>
    </ul>
  </header>
</template>

<script>
export default {
  data() {
    return {
      isMobileMenuShow: false
    };
  },
  mounted() {
    window.addEventListener('scroll',function(){       
      var scrollheight = document.body.scrollTop === 0 ? document.documentElement.scrollTop : document.body.scrollTop;
      var root = document.querySelector('.nav-header')
      var a = document.querySelectorAll('.directory a')
      if(scrollheight > 100) {
        root.style.background = 'rgba(40, 57, 101, .9)'
        for (const item of a) {
          item.style.color = '#fff'
        }
        root.style.transition = 'all 0.2s'
      } else {
        for (const item of a) {
          item.style.color = '#565656'
        }
        root.style.backgroundColor = 'transparent'
        root.style.transition = 'all 0.2s'
      }
    },false);
  },
  methods: {
    showMobileMenu() {
      if (!this.isMobileMenuShow) {
        this.$refs.mobileMenu.style.display = "block";
        this.isMobileMenuShow = true;
      } else {
        this.$refs.mobileMenu.style.display = "none";
        this.isMobileMenuShow = false;
      }
    }
  }
};
</script>
