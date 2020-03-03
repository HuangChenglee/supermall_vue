<template>
  <div id="tabbar">
    <slot></slot>
  </div>
</template>

<script>
  export default {
  };
</script>

<style>
  #tabbar {
    display: flex;
    text-align: center;
    background-color: #f6f6f6;
    position: fixed;
    height: 49px;
    bottom: 0;
    left: 0;
    right: 0;
    box-shadow: 0px -1px 1px rgba(100, 100, 100, 0.08);
    font-size: 14px;
  }
  
</style>