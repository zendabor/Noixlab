<script>
export default {
  name: "DigitalGuide"
}
</script>
<template>
  <section>
    <div class="container">
      <h3 class="DigitalGuide_title">Let us guide You<br> to Digital</h3>
      <span class="DigitalGuide_text text">Our product-driven development<br> combines contemporary trends,<br>business goals and the cutting-edge<br> technology stack.</span>
      <span class="DigitalGuide_desc text">Since 2013, when our team released<br> a first digital project for Milano Fashion Week,<br> we craft high-tech and creativity<br> with top-level partners and clientele.</span>
    </div>
    <div class="background_wrap"></div>
  </section>
</template>
<style scoped>
  section {
    position: relative;
    display: flex;
    align-items: center;
    justify-content: flex-start;
  }
  .background_wrap {
    background-image: url("/src/assets/backgrounds/Group 58726075.png");
    background-size: cover;
    background-repeat: no-repeat;
    position: absolute;
    z-index: -1;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
  }
  .container {
    display: flex;
    flex-direction: column;
    text-align: left;
    gap: 50px;
    width: 50%;
    margin-left: 100px;
    margin-bottom: 150px;
    max-width: 1440px;
  }
  .DigitalGuide_title{
    font-size: 40px;
    line-height: 140%;
    font-weight: bold;
    color: #283534;
  }
  .text br {
    display: none;
  }
  .DigitalGuide_text {
    font-weight: 500;
  }
  .DigitalGuide_desc {
   width: 100%;
  }
  .text {
    font-size: 20px;
    line-height: 140%;
    color: #283534;
  }
  @media (max-width: 420px) {
     section {
       flex-direction: column;
       overflow: hidden;
     }
    .container {
      margin-bottom: 30px;
      margin-top: 50px;
      margin-left: 0;
      width: 100%;
      align-items: center;
    }
    .background_wrap{
      position: unset;
      height: 403px;
      width: 145%;
      background-position: 100%;
      background-size: 218%;
    }
    .DigitalGuide_title {
      font-weight: 700;
      font-size: 24px;
      line-height: 160%;
      width: 100%;
      text-align: center
    }
    .text br {
      display: inline;
    }
    .DigitalGuide_text {
      width: 100%;
      text-align: center;
      font-size: 14px;
      font-weight: 500;
      line-height: 160%;
    }
    .DigitalGuide_desc {
      font-size: 14px;
      font-weight: 500;
      line-height: 160%;
      text-align: center;
    }
  }
</style>
