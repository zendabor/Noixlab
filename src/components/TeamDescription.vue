<script>
import Elipce from "@/components/icons/Elipce.vue";

export default {
  name: "TeamDescription",
  components: {Elipce}
}
</script>
<template>
  <section>
  <div class="container">
    <div class="team_desc">
      <h3 class="team_title">The team of professionals<br>with creative passion in our hearts<br>and your product vision in mind.</h3>
      <div class="desc_wrap">
        <div class="desc_number">9</div>
        <Elipce class="Elipce"></Elipce>
        <span class="desc_text">years with startups,<br>brands & enterprise</span>
      </div>
    </div>
    <ul class="team_list">
      <li class="team_item">
        <div class="img_wrap-blueCycle">
          <img src="/src/assets/img/blueBall.png" alt="">
        </div>
        <div class="item_number">25</div>
        <span class="item_text">Mobile apps released</span>
      </li>
      <li class="team_item">
        <div class="img_wrap-blueCycle">
          <img src="/src/assets/img/blueBall.png" alt="">
        </div>
        <div class="item_number">33</div>
        <span class="item_text">web services integrated</span>
      </li>
      <li class="team_item">
        <div class="img_wrap-blueCycle">
          <img src="/src/assets/img/blueBall.png" alt="">
        </div>
        <div class="item_number">78</div>
        <span class="item_text">designs produced</span>
      </li>
      <li class="team_item">
        <div class="img_wrap-blueCycle">
          <img src="/src/assets/img/blueBall.png" alt="">
        </div>
        <div class="item_number">$10.5m</div>
        <span class="item_text last_item">invested in startups<br> we have worked with</span>
      </li>
    </ul>
    <span class="team_ps">and just uncountable number<br> of all kinds of presentations, slides<br> and pitch decks versions.</span>
  </div>
  </section>
</template>

<style scoped>
  .img_wrap-blueCycle {
    background-color: transparent;
    border-radius: 50%;
    width: 108px;
    height: 108px;
    position: absolute;
    z-index: -1;
    left: -28%;
    top: -26%;
  }
  .Elipce {
    position: absolute;
    top: 13%;
    right: -13%;
    width: 766px;
    z-index: -1;
  }
  section {
    background-color: #F8F8F8;
    overflow: hidden;
    height: 100%;
  }
  .container {
    display: flex;
    flex-direction: column;
    max-width: 1440px;
    position: relative;
    z-index: 1;
    height: 100%;
    margin: 0 auto;
    gap: 110px;
    padding: 259px 100px 186px;
  }
  .team_desc {
    display: flex;
    align-items: center;
    justify-content: space-between;
  }
  .desc_wrap {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 20px;
  }
  .desc_number {
    position: relative;
    font-weight: 700;
    line-height: 160%;
    font-size: 74px;
    padding: 45px;
    border-radius: 50%;
    color: #ffff;
    background-color: #000;
    width: 136px;
    display: flex;
    height: 136px;
    align-items: center;
    justify-content: center;
  }
  .team_title {
    font-size: 40px;
    line-height: 140%;
    color: #283534;
    font-weight: 700;
  }
  .desc_text {
    font-size: 20px;
    line-height: 140%;
    font-weight: bold;
  }
  .desc_wrap{
    display: flex;
  }
  .team_item {
    position: relative;
    z-index: 2;
    gap: 5px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: flex-start;
  }

  .team_item:last-child .img_wrap-blueCycle{
    left: -8%;
  }
  .item_text {
    line-height: 120%;
    font-size: 20px;
    font-weight: 500;
    text-align: start;
  }
  .item_number {
    font-weight: bold;
    font-size: 70px;
    line-height: 120%;
  }
  .team_list {
    display: flex;
    align-items: center;
    justify-content: space-between;
    margin-left: 50px;
  }
  .team_ps {
    font-weight: 500;
    font-size: 20px;
    line-height: 120%;
    color: #283534;
  }
  .team_ps br {
    display: none;
  }
  @media (max-width: 420px){
    .container {
      padding: 60px 0;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      gap: 35px;
    }
    .team_desc {
      flex-direction: column;
      gap: 70px;
      margin-top: 70px;
    }
    .desc_wrap {
      flex-direction: column;
    }
    .team_title {
      width: 100%;
      padding: 0 36px;
      font-size: 24px;
      line-height: 120%;
      text-align: center;
    }
    .Elipce {
      position: absolute;
      top: -17%;
      right: 0;
      rotate: 290deg;
      width: 476px;
      z-index: -1;
    }
    .desc_text {
      text-align: center;
      font-size: 14px;
      line-height: 140%;
      font-weight: bold;
    }
    .item_text {
      font-size: 14px;
      font-weight: 500;
      line-height: 140%;
      text-align: center;
    }
    .last_item {
      width: 55%;
    }
    .img_wrap-blueCycle {
      width: 16px;
      height: 16px;
      position: initial;
    }
    .team_list {
      flex-direction: column;
      gap: 24px;
      margin-left: 0;
    }
    .last_item {
      width: 100%;
    }
    .team_item {
      align-items: center;
    }
    .item_number {
      font-size: 32px;
      line-height: 140%;
      font-weight: 700;
    }
    .team_ps {
      font-size: 14px;
      font-weight: bold;
      line-height: 140%;
      text-align: center;
    }
    .team_ps br {
      display: inline;
    }
  }
</style>
