<template>
  <div>
    <div class="wrapper">
    <myheader></myheader>
      <mycontainer></mycontainer>
    </div>
    <myfooter></myfooter>
  </div>
</template>

<script>
import myheader from "../header";
import mycontainer from "../container";
import myfooter from "../footer";

if (process.browser) {
  // 在这里根据环境引入wow.js
  var { WOW } = require("wowjs");
}

export default {
  components: {
    myheader,
    myfooter,
    mycontainer,
  },
  mounted() {
    if (process.browser) {
      // 在页面mounted生命周期里面 根据环境实例化WOW
      this.$nextTick(() => {
        console.log('okk')
        new WOW({
          live: false,
          offset: 0,
        }).init();
      });
    }
  },
};
</script>

<style lang="stylus" scoped>
.wrapper {
  background: linear-gradient(
    #959595,
    #959595,
    #959595,
    #959595,
    #959595,
    #c5c5c5
  );
  padding-top: 48.6%;
  position: relative;
  padding-bottom: 7%;
  overflow: hidden;
}
</style>