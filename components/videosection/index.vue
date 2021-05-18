<template>
  <div class="section inner">
    <div class="screen-video wow animate__animated animate__fadeInUp">
      <video
        poster="/video/1.jpg"
        src="/video/1.mp4"
        controls
      ></video>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="stylus" scoped>
.screen-video {
  position: relative;

  &::after {
    content: '';
    display: block;
    padding-top: 53.9513%;
    border: solid 1px hotpink;
  }

  video {
    display: block;
    width: 100%;
    height: 100%;
    object-fit: cover;
    position: absolute;
    left: 0;
    top: 0;
    cursor: pointer;
  }
}
</style>