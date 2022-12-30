<script>
import BlackCycle from "@/components/icons/BlackCycle.vue";
import BlueCycle from "@/components/icons/BlueCycle.vue";
import Line from "@/components/icons/Line.vue";
import Subtract from "@/components/icons/Subtract.vue";

export default {
  name: "Noixlab",
  components: {Subtract, Line, BlueCycle, BlackCycle}
}
</script>
<template>
  <section class="section noixlab_section">
    <div class="container">
      <div class="logo_wrap">
        <div class="svg_wrap">
          <BlackCycle class="BlackCycle"></BlackCycle>
          <BlueCycle class="BlueCycle"></BlueCycle>
        </div>
        <h2 class="logo_title">noixlab</h2>
      </div>
      <div class="content_wrapper">
        <div class="text_wrap">
          <span class="text_wrapper">A digital studio from LA with a strong focus on<p> product-driven</p>approach.</span>
          <span class="description">We build UX/UI, presentations,mobile apps & web that really change the game.</span>
        </div>
        <div class="img_wrapper">
          <img src="/src/assets/img/image91.png" alt="">
          <line class="line"></line>
          <Subtract class="Subtract"></Subtract>
          <BlackCycle class="NewBlackCycle"></BlackCycle>
          <BlueCycle class="NewBlueCycle"></BlueCycle>
        </div>
      </div>
    </div>
  </section>
</template>
<style scoped>
.NewBlueCycle {
  position: absolute;
  width: 15px;
  bottom: 42%;
  right: -6%;
}
.NewBlackCycle {
  position: absolute;
  width: 15px;
  bottom: 42%;
  right: -9%;
}
.Subtract {
  position: absolute;
  right: -16%;
  top: 15%;
}
.line {
  position: absolute;
  top: 0;
}
  section {
    display: flex;
    align-items: center;
    overflow: hidden;
  }
  .container {
    width: 100%;
    display: flex;
    flex-direction: column;
  }
  .logo_wrap {
    display: flex;
    gap: 50px;
    align-items: center;
    justify-content: flex-start;
    padding-left: 100px;
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
    width: 70%;
    color: #283534;
    font-weight: 500;
  }
  .text_wrapper {
    width: 60%;
    font-weight: 700;
    font-size: 32px;
    line-height: 160%;
    display: flex;
    flex-direction: column;
    align-items: self-start;
  }
  .text_wrapper p {
    background: -webkit-linear-gradient(#BAF2B5, #26AAD4);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    font-weight: inherit;
  }
  .svg_wrap {
    position: relative;
  }
  .BlueCycle {
    position: absolute;
    top: 28%;
    right: -15px;
  }
  @media (max-width: 420px) {
    .Subtract {
      right: -30%;
    }
    .NewBlueCycle {
      bottom: 15%;
    }
    section {
      padding: 100px 30px 50px;
    }
    .logo_wrap {
      padding: 0;
      margin-bottom: 48px;
    }
    .content_wrapper {
      padding: 0;
      flex-direction: column;
    }
    .text_wrapper {
      font-size: 24px;
      display: flex;
      align-items: center;
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
    .description {
      font-size: 14px;
      margin-bottom: 40px;
      width: 70%;
    }
  }
</style>
