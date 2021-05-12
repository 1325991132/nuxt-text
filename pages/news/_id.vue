<template>
  <div>
    <h1>动态id页面</h1>
    <h2>得到的xid是{{ $route.params.id }}</h2>
    <a href=""><nuxt-link :to="{ name: 'index' }">首页</nuxt-link></a>
  </div>
</template>

<script>
export default {
  validate({params}) {
      console.log(params)
      return params.id === '4567'
  },
  data() {
    return {};
  },
  methods: {},
  mounted(){
      this.$toast.show("曲耀达123")
  }
};
</script>

<style scoped>
</style>