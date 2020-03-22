<template>
  <div id="header">
    <div class="logo-warpper">
      <span class="site-name">有趣导航</span>
    </div>
    <div class="setting-warpper">
      <span class="setting-link">登录</span>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {};
  }
};
</script>

<style scoped>
#header {
  height: 32px;
  border-bottom: 1px solid #ebebeb;
  display: flex;
  justify-content: space-between;
  align-items: center;
  background: #f7f7f7;
}
.logo-warpper,
.setting-warpper {
  height: 32px;
  line-height: 32px;
}
.logo-warpper {
  padding-left: 15px;
}
.site-name {
  font-size: 13px;
  color: #555;
  font-weight: bold;
}
.setting-link {
  font-size: 12px;
  color: #555;
  margin-right: 19px;
  display: inline-block;
  cursor: pointer;
  text-decoration: underline;
}
</style>