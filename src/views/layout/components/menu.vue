<template>
  <div class="menu-list">
        <a-menu
           mode="inline"
           theme="dark"
           :inline-collapsed="$store.state.collapsed">
          <a-menu-item key="1">
             <a-icon type="pie-chart"></a-icon>
             <span>1</span>
          </a-menu-item>
          <a-menu-item key="2">
             <a-icon type="desktop"></a-icon>
             <span>1</span>
          </a-menu-item>
        </a-menu>
  </div>
</template>

<script>
export default {

};
</script>
