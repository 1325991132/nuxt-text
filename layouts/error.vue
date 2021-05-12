<template>
  <div>
    <h1>{{ msg }}</h1>
    <h1>{{error.statusCode}}</h1>
    <h1>{{error.message}}</h1>
    <a href=""><nuxt-link :to="{ name: 'index' }">首页</nuxt-link></a>
  </div>
</template>

<script>
export default {
  props: ["error"],
  data() {
    return {
      msg: "跳转到错误页面",
    };
  },
};
</script>

<style scoped>
</style>