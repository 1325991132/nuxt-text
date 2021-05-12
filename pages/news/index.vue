<template>
  <div>
    <h1>news page</h1>
    <a href=""><nuxt-link :to="{name:'index'}">首页</nuxt-link></a>
    <h2>得到的xid是{{$route.params.xid}}</h2>
    <ul ref="list">
      <li v-for="(item, index) in counst" :key="index">{{ item }}</li>
    </ul>
    <button @click="add">add</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      counst: ["qyd", "nkj", 123],
    };
  },
  methods: {
    add() {
      this.counst.push(Math.random(1, 10));
      this.$nextTick(() => {
        console.log(this.$refs.list.childNodes.length);
      });
    },
  },
};
</script>

<style scoped>
</style>