<template>
  <div id="app">
    <Header />
    <!-- 其他内容 -->
    <router-view></router-view>
  </div>
</template>

<script>
import Header from 'front-page/components/Header.vue'

export default {
  name: 'App',
  components: {
    Header
  }
}
</script>

