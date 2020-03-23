<template>
  <div class="menu-warpper">
    <div class="menu-title-warpper">
      <span class="icon"></span>
      <span class="title">常用</span>
    </div>
    <div class="menu-body-warpper">
      <div class="menu-body menu-item">
        <div class="item">
          <div class="item-icon"></div>
          <div class="item-title">Java</div>
          <div class="item-remark">CSS 提供了 text-indent 属性,该属性可以方便地实现文本缩进。 通过使用 text-indent 属性,所有元素的第一行都可以缩进一个给定的长度,甚至该长度可以是负值。 这个...</div>
        </div>
      </div>
      <div class="menu-body menu-item"></div>
      <div class="menu-body menu-item"></div>
      <div class="menu-body menu-item"></div>
      <div class="menu-body menu-item"></div>
      <div class="menu-body menu-item"></div>
      <div class="menu-body menu-item"></div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
.menu-warpper {
  padding: 10px 25px;
}
.menu-title-warpper {
  height: 20px;
  line-height: 20px;
  margin-bottom: 12px;
}
.icon {
  margin-right: 5px;
}
.title {
  font-size: 13px;
  color: #737373;
  font-weight: bold;
}
.menu-body-warpper {
  display: flex;
  flex-wrap: wrap;
}
.menu-body {
  width: 225px;
  height: 120px;
  cursor: pointer;
  margin: 0 15px 15px 0;
}
.menu-item {
  border-radius: 6px;
  box-shadow: rgba(0, 0, 0, 0.1) 0px 0px 0px 1px inset,
    rgba(12, 12, 13, 0.1) 0px 1px 4px 0px;
  transition: box-shadow 150ms;
}
.menu-item:hover {
  box-shadow: rgba(0, 0, 0, 0.1) 0px 0px 0px 1px inset,
    rgb(215, 215, 219) 0px 0px 0px 5px;
  transition: box-shadow 150ms;
}
.item {
  position: relative;
  height: calc(100% - 20px);
  margin: 10px;
  overflow: hidden;
}
.item-icon {
  background: url(../../assets/nav_cofe.png) no-repeat center;
  background-size: contain;
  width: 35px;
  height: 35px;
  float: left;
  margin-right: 10px;
  border-radius: 50%;
  transition: 0.5s;
}
.menu-item:hover .item-icon {
  transform: rotate(360deg);
}
.item-title {
  height: 35px;
  line-height: 35px;
  font-size: 15px;
  color: #7e7e7e;
  font-weight: 700;
}
.menu-item:hover .item-title {
  color: #ff8300;
}
.item-remark {
  font-size: 12px;
  color: #8c8c8c;
  text-indent: 2em;
  margin-left: 35px;
  line-height: 20px;
}
</style>