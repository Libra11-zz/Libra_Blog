<template>
  <div class="homePage">
    <nav-header></nav-header>
    <div class="home-bg">
      <!-- <mark-down></mark-down> -->
      <div class="introduce">
        <div class="main">
          HI, I AM LIBRA
          <br />WELCOME
        </div>
        <div class="detail">hope you can find what you want</div>
      </div>
    </div>
    <div class="new-book">
      <span class="title">新书推荐</span>
      <ul class="book-list">
        <li>
          <book :bookData="bookData"></book>
        </li>
        <li>
          <book :bookData="bookData"></book>
        </li>
        <li>
          <book :bookData="bookData"></book>
        </li>
        <li>
          <book :bookData="bookData"></book>
        </li>
        <li>
          <book :bookData="bookData"></book>
        </li>
        <li>
          <book :bookData="bookData"></book>
        </li>
        <li>
          <book :bookData="bookData"></book>
        </li>
        <li>
          <book :bookData="bookData"></book>
        </li>
        <li>
          <book :bookData="bookData"></book>
        </li>
        <li>
          <book :bookData="bookData"></book>
        </li>
        <li>
          <book :bookData="bookData"></book>
        </li>
        <li>
          <book :bookData="bookData"></book>
        </li>
        <li>
          <book :bookData="bookData"></book>
        </li>
        <li>
          <book :bookData="bookData"></book>
        </li>
        <li>
          <book :bookData="bookData"></book>
        </li>
        <li>
          <book :bookData="bookData"></book>
        </li>
        <li>
          <book :bookData="bookData"></book>
        </li>
        <li>
          <book :bookData="bookData"></book>
        </li>
      </ul>
    </div>
    <div class="new-blog">
      <span class="title">近期文章</span>
      <ul class="blog-list">
        <li>
          <blog-card></blog-card>
        </li>
        <li>
          <blog-card></blog-card>
        </li>
        <li>
          <blog-card></blog-card>
        </li>
        <li>
          <blog-card></blog-card>
        </li>
        <li>
          <blog-card></blog-card>
        </li>
        <li>
          <blog-card></blog-card>
        </li>
        <li>
          <blog-card></blog-card>
        </li>
        <li>
          <blog-card></blog-card>
        </li>
        <li>
          <blog-card></blog-card>
        </li>
        <li>
          <blog-card></blog-card>
        </li>
        <li>
          <blog-card></blog-card>
        </li>
        <li>
          <blog-card></blog-card>
        </li>
        <li>
          <blog-card></blog-card>
        </li>
        <li>
          <blog-card></blog-card>
        </li>
        <li>
          <blog-card></blog-card>
        </li>
      </ul>
    </div>
    <div class="hot-book">
      <span class="title">热门书籍</span>
      <ul class="book-list">
        <li>
          <book :bookData="bookData"></book>
        </li>
        <li>
          <book :bookData="bookData"></book>
        </li>
        <li>
          <book :bookData="bookData"></book>
        </li>
        <li>
          <book :bookData="bookData"></book>
        </li>
        <li>
          <book :bookData="bookData"></book>
        </li>
        <li>
          <book :bookData="bookData"></book>
        </li>
        <li>
          <book :bookData="bookData"></book>
        </li>
        <li>
          <book :bookData="bookData"></book>
        </li>
        <li>
          <book :bookData="bookData"></book>
        </li>
        <li>
          <book :bookData="bookData"></book>
        </li>
        <li>
          <book :bookData="bookData"></book>
        </li>
        <li>
          <book :bookData="bookData"></book>
        </li>
        <li>
          <book :bookData="bookData"></book>
        </li>
        <li>
          <book :bookData="bookData"></book>
        </li>
        <li>
          <book :bookData="bookData"></book>
        </li>
        <li>
          <book :bookData="bookData"></book>
        </li>
        <li>
          <book :bookData="bookData"></book>
        </li>
        <li>
          <book :bookData="bookData"></book>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
import navHeader from "@/components/nav-header";
import book from "@/components/book";
import blogCard from "@/components/blog-card";
export default {
  data() {
    return {
      bookData: {
        name: "libra",
        author: "Libra",
        describe: "dlkjfsldjfsldkjflsdkjf"
      }
    };
  },
  components: {
    navHeader,
    book,
    blogCard
  }
};
</script>

<style lang="less">
@import "./index.less";
</style>
