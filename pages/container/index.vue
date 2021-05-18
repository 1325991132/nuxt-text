<template>
  <div class="container wrapper-main">
      <div class="home">
          <mynavbar></mynavbar>
          <myvideosection></myvideosection>
          <homepart2></homepart2>
          <homepart3></homepart3>
      </div>
  </div>
</template>

<script>
import mynavbar from '@/components/navbar'
import myvideosection from '@/components/videosection'
import homepart2 from '@/components/homepart2'
import homepart3 from '@/components/homepart3'

export default {
    components: {
        mynavbar,
        myvideosection,
        homepart2,
        homepart3
    },
};
</script>

<style lang="stylus" scoped>
.container {
  width: 96%;
  max-width: 1500px;
  margin: 0 auto;
}

.wrapper-main {
  background: linear-gradient(0deg, #272727, #010000, #414042, #010000, #3b3b3b);
  box-shadow: 0 20px 52px 10px rgba(26, 22, 23, 0.75);
  padding-bottom: 180px;
  position: relative;
  z-index: 1;
  min-height: 800px;
}
</style>