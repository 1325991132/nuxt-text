<template>
  <div class="footer">
    <img src="/picture/bottom_bg.jpg" width="100%" />
    <div class="logo">
      <img
        src="/picture/logo.png"
        class="wow animate__animated animate__rubberBand"
      />
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="stylus" scoped>
.footer {
  position: relative;

  .logo {
    position: absolute;
    left: 50%;
    bottom: 18%;
    -webkit-transform: translateX(-50%);
    transform: translateX(-50%);
    max-width: 40%;
  }
}
</style>