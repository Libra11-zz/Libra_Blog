<template>
  <div class='book'>
    <chart />
    <chart />
    <chart />
    <chart />
    <chart />
  </div>
</template>

<script>
import chart from "@/components/chart";
  export default {
    components: {
      chart
    }
  }
</script>

<style lang="less" scoped>
.book{
  background:#fff;
}
</style>