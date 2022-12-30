<script>
export default {
  name: "DigitalGuide"
}
</script>
<template>
  <section>
    <div class="container">
      <h3 class="DigitalGuide_title">
        Let us guide You to Digital
      </h3>
      <span class="DigitalGuide_text text">Our product-driven development combines contemporary trends,business goals and the cutting-edge technology stack.</span>
      <span class="DigitalGuide_desc text">Since 2013, when our team released a first digital project for Milano Fashion Week, we craft high-tech and creativity with top-level partners and clientele.</span>
    </div>
  </section>
</template>
<style scoped>
  section {
    background-image: url("/src/assets/backgrounds/Group 58726075.png");
    background-size: cover;
    background-repeat: no-repeat;
    display: flex;
    align-items: center;
    justify-content: flex-start;
  }
  .container {
    display: flex;
    flex-direction: column;
    text-align: left;
    gap: 50px;
    width: 50%;
    margin-left: 100px;
    margin-bottom: 150px;
  }
  .DigitalGuide_title{
    font-size: 40px;
    line-height: 140%;
    font-weight: bold;
    color: #283534;
  }
  .DigitalGuide_text {
    font-weight: bold;
  }
  .DigitalGuide_desc {
    width: 70%;
  }
  .text {
    font-size: 20px;
    line-height: 28px;
    color: #283534;
  }
  @media (max-width: 420px) {
    .container {
      margin-top: 50px;
      margin-left: 0;
      width: 100%;
      align-items: center;
    }
    .DigitalGuide_title {
      width: 80%;
      text-align: center
    }
    .DigitalGuide_text {
      width: 78%;
      text-align: center;
    }
    .DigitalGuide_desc {
      width: 86%;
      text-align: center;
    }
  }
</style>
