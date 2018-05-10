<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style>
  * {
    margin: 0;
    padding: 0;
  }
  body {
    background-color: #e2e2e2;
  }
  /* 隐藏滚动条，未做兼容处理 */
  ::-webkit-scrollbar {
  	display:none;
  }
</style>
