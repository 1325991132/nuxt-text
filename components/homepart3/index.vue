<template>
  <section class="section home-part3" id="">
    <div class="column-title wow animate__animated animate__fadeInUp">
      <span class="en-txt">BUSINESS STRUCTURE</span>
      <span class="cn-txt">业务架构</span>
    </div>
    <div class="label-bar wow animate__animated animate__fadeInUp">
      <div class="list" id="labelList">
        <div class="item">
          <img src="/picture/pic_05_06.png" class="icon" />
          <span class="cn-txt">体育赛事</span>
          <span class="en-txt">SPORTS EVENTS</span>
        </div>
        <div class="item">
          <img src="/picture/pic_05_04.png" class="icon" />
          <span class="cn-txt">展览展示</span>
          <span class="en-txt">EXHIBITION</span>
        </div>
        <div class="item">
          <img src="/picture/pic_05_02.png" class="icon" />
          <span class="cn-txt">电子竞技</span>
          <span class="en-txt">E-SPORTS</span>
        </div>
        <div class="item">
          <img src="/picture/pic_05_03.png" class="icon" />
          <span class="cn-txt">娱乐晚会</span>
          <span class="en-txt">ENTERTAINMENT</span>
        </div>
        <div class="item">
          <img src="/picture/pic_05_01.png" class="icon" />
          <span class="cn-txt">企业宣传</span>
          <span class="en-txt">ENTERPRISE PROPAGANDA</span>
        </div>
        <div class="item">
          <img src="/picture/pic_05_05.png" class="icon" />
          <span class="cn-txt">新闻报道</span>
          <span class="en-txt">NEWS REPORT</span>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style lang="stylus" scoped>
.home-part3 {
  background: url('/images/bg_business.png') no-repeat top;
  padding-bottom: 7.8%;
  padding-top: 18.5%;
  margin-top: 30px;

  .column-title {
    margin-bottom: 30px;
  }

  .label-bar {
    background-color: rgba(0, 0, 0, 0.62);
    color: #dd9d26;
    text-align: center;
    padding: 15px 3.6%;

    .item .icon {
      display: block;
      margin: 0 auto;
    }

    .cn-txt {
      display: block;
      font-size: 20px;
      margin: 4px 0;
    }

    .en-txt {
      display: block;
      font-size: 16px;
    }

    .slick-dots {
      font-size: 0;
      text-align: center;
      margin-top: 30px;

      li {
        display: inline-block;
        vertical-align: top;
        margin: 0 4px;
        width: 8px;
        height: 8px;
        background-color: rgba(255, 255, 255, 0.5);
        border-radius: 50%;

        slick-active {
          background-color: #dd9d26;
        }

        button {
          display: none;
        }
      }
    }
  }
}
</style>