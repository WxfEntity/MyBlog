<template>
  <div>
    <el-menu
      :default-active="activeIndex2"
      class="el-menu-demo"
      mode="horizontal"
      @select="handleSelect"
      background-color="#1e5d64"
      text-color="#fff"
      active-text-color="#ffd04b">
      <el-menu-item index="1" class="menus">首页</el-menu-item>
      <el-menu-item index="2"  class="menus">文章列表</el-menu-item>
      <el-menu-item index="3"  class="menus">最热文章</el-menu-item>
      <el-menu-item index="4" class="menus"><a href="" target="_blank">订单管理</a></el-menu-item>
      <!--<input class="input"></input>-->
    </el-menu>
  </div>
</template>

<script>
  import Input from './Input.vue'
  export default {
    components: {Input},
    data() {
      return {
        activeIndex: '1',
        activeIndex2: '1'
      };
    },
    methods: {
      handleSelect(key, keyPath) {
        console.log(key, keyPath);
      }
    }
  }
</script>

<style scoped>
.menus{
  float:left;
  left: 30%;
}
  .input{
    position: absolute;
    top: 20px;
    left: 50%;
  }
</style>
