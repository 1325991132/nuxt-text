<template>
  <div class="navbar">
    <ul class="navlist inner clearfix">
      <li class="item wow animate__animated animate__fadeInDown">
        <a href="#AboutUs">
          <span class="cn-txt">公司介绍</span>
          <span class="en-txt">ABOUT US</span>
        </a>
      </li>
      <li class="item wow animate__animated animate__fadeInDown" data-wow-delay="0.5s">
        <a href="#ClassicCase">
          <span class="cn-txt">精品案例</span>
          <span class="en-txt">CLASSIC CASE</span>
        </a>
      </li>
      <li class="item wow animate__animated animate__fadeInDown" data-wow-delay="1s">
        <a href="#Team">
          <span class="cn-txt">公司团队</span>
          <span class="en-txt">TEAM</span>
        </a>
      </li>
      <li class="item wow animate__animated animate__fadeInDown" data-wow-delay="1.5s">
        <a href="#Partner">
          <span class="cn-txt">合作企业</span>
          <span class="en-txt">PARTNER</span>
        </a>
      </li>
      <li class="item wow animate__animated animate__fadeInDown" data-wow-delay="2s">
        <a href="#ContactUs">
          <span class="cn-txt">联系我们</span>
          <span class="en-txt">CONTACT US</span>
        </a>
      </li>
    </ul>
  </div>
</template>

<script>
export default {};
</script>

<style lang="stylus" scoped>
.navbar {
  padding: 62px 0 24px;
  margin-bottom: 2%;

  .navlist {
    display: flex;
    justify-content: space-around;
    width: 100%;
  }

  .navlist::after, .navlist::before {
    content: '';
    display: inline-block;
    vertical-align: top;
  }

  .inner {
    padding: 20px 0;
  }

  .item {
    display: inline-block;
    vertical-align: top;
    text-align: center;

    a {
      display: inline-block;
    }

    span {
      display: block;
      line-height: 120%;
    }

    .cn-txt {
      color: #fff;
      font-size: 30px;
      font-weight: 700;
    }

    .en-txt {
      color: #f18900;
      font-size: 22px;
      text-transform: uppercase;
      margin-top: 7px;
    }
  }
}
</style>