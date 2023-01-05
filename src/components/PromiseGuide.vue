<script>
import Earth from "@/components/icons/Earth.vue";

export default {
  name: "PromiseGuide",
  components: {Earth}
}
</script>
<template>
  <section>
    <div class="PromiseGuide_container">
      <h2 class="PromiseGuide_title">We create the world-class products
        <p>in digital field.</p></h2>
      <div class="PromiseGuide_btn">
        <span class="PromiseGuide_btn-text">We support startups around the world 🚀</span>
        <div class="svg_wrap"><Earth></Earth></div>
      </div>
      <ul class="PromiseGuide_list">
        <li class="PromiseGuide_item">
          <span class="item_title">UI/UX Design</span>
          <div class="text_wrap">
            <span class="item_text">Mobile & Wearables</span>
            <span class="item_text">Web Design</span>
          </div>
        </li>
        <li class="PromiseGuide_item">
          <span class="item_title">Mobile Apps</span>
          <div class="text_wrap">
            <span class="item_text">iOS & Android apps</span>
            <span class="item_text">Tablets and Wearables</span>
          </div>
        </li>
        <li class="PromiseGuide_item">
          <span class="item_title">Web</span>
          <div class="text_wrap">
            <span class="item_text">Web Pages</span>
            <span class="item_text">CRM/ERP Solutions</span>
          </div>
        </li>
        <li class="PromiseGuide_item">
          <span class="item_title">Presentations</span>
          <div class="text_wrap">
            <span class="item_text">Pitch Decks</span>
            <span class="item_text">Event Presentations</span>
          </div>
        </li>
      </ul>
    </div>
  </section>
</template>

<style scoped>
  section {
    height: 100vh;
    background-color: #0F1515;
  }
  .PromiseGuide_container {
    position: relative;
    padding: 10% 5% 2%;
    align-items: self-start;
    height: 100%;
    gap: 20% 0;
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    grid-template-rows: repeat(2,1fr);
    grid-template-areas:
    "a a b"
    "c c c";
  }
  .PromiseGuide_container:after {
    content: '';
    position: absolute;
    width: 100%;
    height: 100%;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background-image: url("/src/assets/backgrounds/c324b6fe7eadb556d11615a929638459.png");
    opacity: 0.4;
    pointer-events: none;
  }
  .PromiseGuide_title {
    grid-area: a;
    color: #ffff;
    font-weight: 700;
    font-size: 40px;
    line-height: 140%;
  }
  .PromiseGuide_title p {
    background: -webkit-linear-gradient(#BAF2B5, #26AAD4);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    font-style: inherit;
    font-weight: inherit;
    font-size: inherit;
    line-height: inherit;
  }
  .PromiseGuide_btn {
    grid-area: b;
    background-color: rgba(255, 255, 255, 0.1);
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 20px 15px 20px 50px;
  }
  .PromiseGuide_btn-text {
    width: 42%;
    text-align: start;
    font-weight: 500;
    font-size: 16px;
    line-height: 140%;
    color: #ffff;
  }
  .svg_wrap {
    padding: 5px;
    background-color: #1E201F;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
  }
  .PromiseGuide_list {
    grid-area: c;
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 0;
  }
  .PromiseGuide_item {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: center;
  }
  .text_wrap {
    display: flex;
    flex-direction: column;
  }
  .item_title {
    font-weight: 700;
    font-size: 24px;
    line-height: 120%;
    color: #ffff;
    margin-bottom: 20px;
  }
  .item_text {
    font-weight: 400;
    font-size: 20px;
    line-height: 120%;
    color: #ffff;
    margin-bottom: 15px;
  }
  .item_text:last-child{
    margin-bottom: 0;
  }
  @media (max-width:420px) {
    .PromiseGuide_container {
      gap: 32px;
      padding: 56px 24px 90px;
      display: grid;
      grid-template-columns: 1fr;
      grid-template-rows:1fr;
      grid-template-areas:
    "a"
    "c"
    "b";
    }
    .PromiseGuide_list {
      align-items: self-start;
      flex-direction: column;
      gap: 20px;
    }
    .PromiseGuide_title {
      font-size: 20px;
    }
    .item_text:first-child {
      margin-bottom: 0;
      margin-right: 15px;
    }
    .text_wrap {
      flex-direction: row;
    }
    .item_title {
      font-size: 14px;
      line-height: 120%;
    }
    .item_text {
      font-size: 14px;
    }
    .PromiseGuide_btn {
      padding: 8px 16px;
    }
    .PromiseGuide_btn-text {
      width: 59%;
      font-size: 14px;
      line-height: 140%;
    }
  }
</style>
