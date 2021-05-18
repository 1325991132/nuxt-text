<template>
  <div class="container">
    <mylayout></mylayout>
    <!-- <div>
      <Logo />
      <h1>nuxt project</h1>
      <ul>
        <li><nuxt-link :to="{name:'about',query:{id:456}}">about</nuxt-link></li>
        <li><nuxt-link :to="{name:'news',params:{xid:123}}">news</nuxt-link></li>
        <li><nuxt-link :to="{name:'test',params:{xid:123}}">test</nuxt-link></li>
        <li><a href="/news/4567">动态路由</a></li>
        <li><nuxt-link :to="{name:'err',params:{xid:123}}">跳转到错误页面</nuxt-link></li>
      </ul>
    </div> -->
  </div>
</template>

<script>
import mylayout from './layout/index.vue'
export default {
  components: {
    mylayout,
  },
};
</script>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont,
    "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

</style>
