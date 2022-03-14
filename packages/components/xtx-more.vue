<template>
  <router-link :to="path" class="xtx-more">
    <span>查看全部</span>
    <i class="iconfont icon-angle-right"></i>
  </router-link>
</template>

<script>
export default {
  name: "XtxMore",
  props: {
    path: {
      type: String,
      default: "/",
    },
  },
};
</script>

<style scoped lang="less">
.xtx-more {
  margin-bottom: 2px;
  display: flex;
  span {
    font-size: 16px;
    vertical-align: middle;
    margin-right: 4px;
    color: #999;
  }
  i {
    font-size: 14px;
    vertical-align: middle;
    color: #ccc;
  }
  &:hover {
    span,
    i {
      color: var(--xtx-color);
    }
  }
}
</style>
