<script>
import BlueCycle from "@/components/icons/BlueCycle.vue";
import Reactrangle from "@/components/icons/Reactrangle.vue";
import Subtract from "@/components/icons/Subtract.vue";
import Elipce from "@/components/icons/Elipce.vue";

export default {
  name: "TeamDescription",
  components: {Elipce, Subtract, Reactrangle, BlueCycle}
}
</script>
<template>
  <section>
    <div class="team_desc">
      <h3 class="team_title">The team of professionals with creative passion in our hearts and your product vision in mind.</h3>
      <div class="desc_wrap">
        <div class="desc_number">9</div>
        <span class="desc_text">years with startups,brands & enterprise</span>
      </div>
    </div>
    <ul class="team_list">
      <li class="team_item">
        <BlueCycle class="BlueCycle"></BlueCycle>
        <div class="item_number">25</div>
        <span class="item_text">Mobile apps released</span>
      </li>
      <li class="team_item">
        <BlueCycle class="BlueCycle"></BlueCycle>
        <div class="item_number">33</div>
        <span class="item_text">web services integrated</span>
      </li>
      <li class="team_item">
        <BlueCycle class="BlueCycle"></BlueCycle>
        <div class="item_number">78</div>
        <span class="item_text">designs produced</span>
      </li>
      <li class="team_item">
        <BlueCycle class="BlueCycle"></BlueCycle>
        <div class="item_number">$10.5m</div>
        <span class="item_text">invested in startups we have worked with</span>
      </li>
    </ul>
    <span class="team_ps">and just uncountable number of all kinds of presentations, slides and pitch decks versions.</span>
    <Elipce class="Elipce"></Elipce>
  </section>
</template>

<style scoped>
  .Elipce {
    position: absolute;
    top: 9%;
    right: -5%;
    width: 766px;
    z-index: -1;
  }
  section {
    padding: 184px 100px;
    position: relative;
    background-color: #F8F8F8;
    z-index: 1;
    overflow: hidden;
    height: 100%;
  }
  .team_title {
    width: 100%;
  }
  .team_desc {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 160px;
    margin-bottom: 160px;
  }
  .desc_wrap {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 20px;
  }
  .desc_number {
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
    width: 50%;
  }
  .desc_text {
    font-size: 20px;
    line-height: 140%;
    width: 50%;
  }
  .desc_wrap{
    display: flex;
  }
  .team_item {
    position: relative;
    z-index: 2;
    gap: 10px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: flex-start;
  }
  .BlueCycle {
    width: 108px;
    height: 108px;
    position: absolute;
    z-index: -1;
    left: -28%;
    top: -14%;
  }
  .team_item:last-child .BlueCycle{
    left: -8%;
  }
  .item_text {
    line-height: 120%;
    font-size: 20px;
    font-weight: 500;
  }
  .item_number {
    font-weight: bold;
    font-size: 70px;
    line-height: 120%;
  }
  .team_list {
    display: flex;
    align-items: center;
    justify-content: space-around;
    margin-bottom: 80px;
  }
  .team_ps {
    font-weight: 500;
    font-size: 20px;
    line-height: 120%;
    color: #283534;
  }
  @media (max-width: 420px){
    section{
      display: none;
    }
  }
</style>
