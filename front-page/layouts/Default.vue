<template>
    <div>
      <!-- 头部组件 -->
      <header>
        <!-- 这里可以放置导航栏等内容 -->
      </header>
  
      <!-- 页面主体内容 -->
      <main>
        <slot />
      </main>
  
      <!-- 页脚组件 -->
      <Footer />
    </div>
  </template>
  
  <script setup>
  import Footer from 'front-page/components/Footer.vue'
  </script>
  
  <style>
  /* 这里可以添加全局样式 */
  </style>