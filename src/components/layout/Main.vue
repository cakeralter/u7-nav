<template>
  <div id="main">
    <main>
      <div class="top">
        <div class="search-warpper">
          <img src="../../assets/nav_google.png" alt="Google" class="search-nav-img left" />
          <input type="text" class="search-ipt-txt" placeholder="点击左侧图标可选择搜索引擎；按回车搜索" />
          <img src="../../assets/nav_btn.png" alt="搜索" class="search-nav-img right" />
        </div>
      </div>
      <div class="center">
        <Menu />
        <Menu />
        <Menu />
        <Menu />
      </div>
    </main>
  </div>
</template>

<script>
import Menu from "../common/Menu";
export default {
  data() {
    return {};
  },
  components: {
    Menu
  }
};
</script>

<style scoped>
#main {
  min-height: calc(100vh - 95px);
  padding: 30px 32px 32px;
}
main {
  width: 1024px;
  margin: auto;
}
.top {
  padding: 0 25px;
}
.search-warpper {
  padding-bottom: 60px;
  width: 736px;
  min-height: 50px;
  margin: auto;
  position: relative;
}
.search-nav-img {
  position: absolute;
  top: 10px;
  width: 30px;
}
.left {
  left: 10px;
}
.right {
  right: 10px;
  cursor: pointer;
}
.search-ipt-txt {
  width: calc(100% - 102px);
  font-size: 15px;
  box-shadow: 0 1px 4px 0 rgba(12, 12, 13, 0.2), 0 0 0 1px rgba(0, 0, 0, 0.15);
  border-radius: 5px;
  border: 1px solid #e6e6e6;
  line-height: 50px;
  padding: 0 50px;
  color: #999;
}
.search-ipt-txt:focus {
  border: 1px solid #2188ff;
  box-shadow: 0 0 5px 0px rgba(71, 158, 245, 0.5);
}
</style>