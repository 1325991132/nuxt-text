<template>
  <div class="header">
    <img src="/picture/top_bg.jpg" />
    <div class="logo">
      <img
        src="/picture/logo.png"
        class="wow animate__animated animate__zoomInUp"
      />
    </div>
  </div>
</template>

<script>

</script>

<style lang="stylus" scoped>
.header {
  position: absolute;
  left: 0;
  top: 0;
  width: 100%;

  .logo {
    position: absolute;
    left: 50%;
    top: 5%;
    -webkit-transform: translateX(-50%);
    transform: translateX(-50%);
    max-width: 40%;
  }
}
</style>