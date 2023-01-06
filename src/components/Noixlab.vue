<script>
import BlackCycle from "@/components/icons/BlackCycle.vue";
import GraphTop from "@/components/icons/GraphTop.vue";

export default {
  name: "Noixlab",
  components: {GraphTop, BlackCycle}
}
</script>
<template>
  <section>
    <div class="container">
      <div class="logo_wrap">
        <div class="svg_wrap">
          <BlackCycle class="BlackCycle"></BlackCycle>
        </div>
        <h2 class="logo_title">noixlab</h2>
      </div>
      <div class="content_wrapper">
        <div class="text_wrap">
          <div class="text_wrapper">A digital studio from LA<br> with a strong focus on<br><span> product-driven</span> approach.</div>
          <span class="description description-desktop">We build UI/UX, Mobile Apps & Web, Presentations<br> that really change the game.</span>
          <span class="description description-mobile">We build UX/UI, presentations,<br>mobile apps & web<br> that really change the game.</span>
        </div>
        <div class="img_wrapper">
          <img src="/src/assets/img/image91.png" alt="">
            <GraphTop class="GraphTop"></GraphTop>
        </div>
      </div>
    </div>
  </section>
</template>
<style scoped>
    .description-mobile {
      display: none;
    }
  .GraphTop {
    position: absolute;
    top: 5%;
    right: -18%;
  }
  .BlackCycle {
    fill: black;
  }
  section {
    display: flex;
    align-items: center;
    overflow: hidden;
  }
  .container {
    display: flex;
    flex-direction: column;
    align-items: center;
    width: 100%;
    justify-content: center;
    max-width: 1440px;
    margin: 0 auto;
  }
  .logo_wrap {
    display: flex;
    gap: 50px;
    align-items: center;
    justify-content: flex-start;
    padding-left: 100px;
    width: 100%;
  }
  .img_wrapper {
    position: relative;
  }
  .content_wrapper {
    display: flex;
    align-items: center;
    width: 100%;
    justify-content: space-between;
    padding: 0 100px;
  }
  .logo_title {
    font-weight: 300;
    font-size: 60px;
    font-family: Geometria;
  }
  .text_wrap {
    width: 52%;
    display: flex;
    flex-direction: column;
    gap: 50px;
  }
  .description {
    font-size: 20px;
    line-height: 160%;
    color: #283534;
    font-weight: 500;
  }
  .text_wrapper {
    font-weight: 700;
    font-size: 32px;
    line-height: 160%;
    display: inline;
  }
  .text_wrapper span {
    background: -webkit-linear-gradient(#BAF2B5, #26AAD4);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    font-weight: inherit;
  }
  .svg_wrap {
    position: relative;
  }
  @media (max-width: 420px) {
    section {
      padding: 90px 30px;
    }
    .GraphTop {
      width: 75px;
      top: -25%;
    }
    .description-mobile {
      display: inline;
    }
    .description-desktop {
      display: none;
    }
    .logo_title {
      font-size: 30px;
    }
    section {
      padding: 100px 30px 90px;
    }
    .logo_wrap {
      padding: 0;
      margin-bottom: 48px;
      justify-content: center;
      gap: 20px;
    }
    .content_wrapper {
      padding: 0;
      flex-direction: column;
      align-items: start;
    }
    .text_wrapper {
      font-size: 24px;
    }
    .text_wrapper,.text_wrap{
      width: 100%;
    }
    .text_wrap {
      justify-content: center;
      align-items: center;
      text-align: center;
      gap: 32px;
    }
    .img_wrapper {
      width: 260px;
    }
    .description {
      font-size: 14px;
      margin-bottom: 40px;
      font-weight: 400;
      line-height: 200%;
    }
  }
</style>
