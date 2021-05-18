<template>
  <div>
    about page
    <h2>接收到route.query为{{ $route.query.id }}</h2>
    <a href=""><nuxt-link :to="{ name: 'index' }">首页</nuxt-link></a>
    <p>标题：{{ info.title }}</p>
    <p>描述：{{ info.desc }}</p>
  </div>
</template>
<script>
import axios from "axios";

export default {
  transition: "about",
  asyncData(ctx) {
    return axios({
      methods: "get",
      url: "/tempData.json",
    })
      .then((_data) => {
        console.log(_data);
        return { info: _data.data.data };
      })
      .catch((err) => {
        console.log(err.response);
        ctx.error({
          statusCode: err.response.status,
          message: err.response.statusText,
        });
      });
  },
  head() {
    return {
      title: this.info.msg,
    };
  },
  data() {
    return {};
  },
};
</script>

<style lang="stylus" scoped>
h2 {
  color: $default-color;
}
</style>