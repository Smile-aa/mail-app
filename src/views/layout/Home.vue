<template>
  <div class="home">

         <div class="menu-list">
           <a-menu  mode="inline" theme="dark" :inline-collapsed="collapsed">
             <a-menu-item key="1">
             <a-icon type="pie-chart"></a-icon>
             <span>1</span>
           </a-menu-item>
           </a-menu>
         </div>

    <div :class="{'main-app': true, 'menu-unfold': collapsed}">
       <div class="main-header">
         <a-button type="primary" style="margin-bottom: 16px" @click="toggleCollapsed">
            <a-icon :type="collapsed ? 'menu-unfold' : 'menu-fold'" />
      </a-button>
    <div class="breadcrumb">
       <a-breadcrumb>
    <a-breadcrumb-item>首页</a-breadcrumb-item>
    <a-breadcrumb-item><a href=""> 统计</a></a-breadcrumb-item>
  </a-breadcrumb>
    </div>
    <ul class="user-info">
      <li>欢迎user
        <a-icon type="down" />
      </li>
      <li>退出</li>
    </ul>
    </div>
  </div>
  </div>
</template>

<script>

export default {
  data() {
    return {
      collapsed: false,
    };
  },
  methods: {
    toggleCollapsed() {
      this.collapsed = !this.collapsed;
    },
  },
};
</script>

<style lang="less">
@import url("~@/assets/css/home.less");
</style>
