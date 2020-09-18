<template>
<!-- 定义组件模板 -->
  <div id="app">
    <Layout></Layout>
  </div>
</template>

<script>
// 定义组件逻辑

// 2.引入组件

import Layout from "./components/Layout"


// 最后一定要暴露一个配置对象
export default {
  name: 'App',
  // 定义App 的子组件
  components: {
      Layout
  }
}
</script>

<style>
html,body,#app,.layout{
  height: 100%;
}
</style>
