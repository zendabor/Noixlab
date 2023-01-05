<script>
import ZigZag from "@/components/icons/ZigZag.vue";
import Subtract from "@/components/icons/Subtract.vue";
import Reactrangle from "@/components/icons/Reactrangle.vue";
import BlackCycle from "@/components/icons/BlackCycle.vue";
import BlueCycle from "@/components/icons/BlueCycle.vue";

export default {
  name: "CompanyContacts",
  components: {BlueCycle, BlackCycle, Reactrangle, Subtract, ZigZag}
}
</script>
<template>
  <section>
    <div class="container">
      <div class="img_wrap">
        <img src="/src/assets/img/image726.png" alt="">
        <BlueCycle class="BlueCycle"></BlueCycle>
        <BlackCycle class="BlackCycle"></BlackCycle>
        <Reactrangle class="Reactrangle"></Reactrangle>
        <ZigZag class="ZigZag"></ZigZag>
      </div>
      <div class="contact_wrap">
        <h3 class="contact_title">Let’s Talk</h3>
        <a href="mailto:hi@noixlab.com" type="email" class="contact_email">hi@noixlab.com</a>
      </div>
      <ul class="contact_list">
        <li class="contact_item">
          <a href="" class="contact_soc">Twitter</a>
        </li>
        <li class="contact_item">
          <a href="" class="contact_soc">Medium</a>
        </li>
        <li class="contact_item">
          <a href="" class="contact_soc">Facebook</a>
        </li>
        <li class="contact_item">
          <a href="" class="contact_soc">Dribbble</a>
        </li>
      </ul>
      <address>13333 Saticoy, suite #1 North Hollywood, CA 91605</address>
      <div class="priv_pol">© 2022 Noixlab.<span>Privacy policy</span></div>
    </div>
  </section>
</template>

<style scoped>
  section {
    height: 100%;
    position: relative;
    padding: 100px 100px 70px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    background-image: url("/src/assets/img/image92.png");
    background-repeat: no-repeat;
    background-size: contain;
  }
  .container {
    width: 100%;
    height: 100%;
    /*display: flex;*/
    /*align-items: center;*/
    /*justify-content: space-evenly;*/
    display: grid;
    align-items: center;
    justify-items: end;
    grid-gap: 0 17%;
    grid-template-columns: 1fr 0.7fr;
    grid-template-rows: repeat(6,.5fr);
    grid-template-areas:
    'img title'
    'img social_media'
    'img address'
    'img policy';
  }
  .contact_wrap {
    grid-area: title;
    display: flex;
    flex-direction: column;
    gap: 20px;
    align-items: flex-end;
    grid-row-start: 2;
    margin-bottom: 30px;
  }
  .contact_list {
    display: flex;
    gap: 20px 80px;
    width: 76%;
    flex-wrap: wrap;
    align-items: center;
    justify-content: flex-end;
    grid-area: social_media;
    grid-row-start: 3;
  }
  .contact_item{
    position: relative;
    flex: 1;
    text-align: end;
  }
  .contact_item:hover::before{
    content: "";
    position: absolute;
    bottom: 0;
    right: 0;
    background: linear-gradient(rgba(186, 242, 181, 0.5),rgba(38, 170, 212, 0.5));
    height: 3px;
    width: 100%;
  }
  .contact_title{
    font-size: 60px;
    line-height: 120%;
    font-weight: 800;
    letter-spacing: -4px;
  }
  .contact_email{
    font-size: 40px;
    line-height: 120%;
    position: relative;
    font-weight: 600;
  }
  .contact_email:before {
    content: "";
    position: absolute;
    bottom: 0;
    right: 0;
    background: black;
    height: 2px;
    width: 100%;
  }
  .contact_email:hover::before{
    background: linear-gradient(rgba(186, 242, 181, 0.5),rgba(38, 170, 212, 0.5));
  }
  .contact_soc {
    font-size: 20px;
    line-height: 120%;
  }
  address {
    font-size: 20px;
    line-height: 120%;
    width: 55%;
    grid-area: address;
    grid-row-start: 4;
    text-align: end;
  }
  .img_wrap {
    position: relative;
    grid-area: img;
    grid-row-start: 1;
    grid-row-end: 7;
  }
  .priv_pol {
    grid-area: policy;
    grid-row-start: 5;
    font-size: 20px;
    line-height: 120%;
    font-weight: 400;
  }
  .ZigZag,.Reactrangle,.BlueCycle,.BlackCycle {
    position: absolute;
  }
  .BlueCycle,.BlackCycle {
    width: 121px;
    height: 121px;
  }
  .BlackCycle {
    right: -13%;
    top: 6%;
    fill: #283534;
  }
  .BlueCycle {
    right: -15%;
    top: 5%;
  }
  .ZigZag {
    top: 21%;
    right: -23%;
  }
  .Reactrangle {
    top: 17%;
    right: -26%;
  }
  .priv_pol span {
    border-bottom: 2px solid black;
  }
  @media (max-width:420px) {
    section {
      padding: 40px 52px 46px;
      background-image: none;
      overflow: hidden;
    }
    .container{
      display: grid;
      align-items: center;
      justify-items: center;
      grid-gap: 24px;
      grid-template-columns: 1fr;
      grid-template-rows: repeat(5,min-content);
      justify-content: center;
      grid-template-areas:
        'title'
        'address'
        'img'
        'social_media'
        'policy';
    }
    .contact_title {
      grid-row-start: 1;
    }
    .contact_list {
      grid-row-start: 4;
    }
    .priv_pol {
      grid-row-start: 5;
    }
    .ZigZag,.Reactrangle,.BlueCycle,.BlackCycle {
      display: none;
    }
    .img_wrap {
      max-width: 330px;
      overflow: hidden;
      max-height: 198px;
      display: flex;
      align-items: center;
      justify-content: center;
      grid-row-start: 3;
      grid-row-end: 3;
    }
    .img_wrap img {
      width: 120%;
      height: 100%;
    }
    .contact_wrap {
      flex-direction: column;
      align-items: center;
      justify-content: center;
      text-align: center;
      gap: 32px;
      grid-row-start: 1;
    }
    .contact_list {
      flex-wrap: nowrap;
      flex-direction: row;
      width: 100%;
      gap: 0 20px;
      align-items: center;
      justify-content: space-between;
    }
    address {
      width: 83%;
      text-align: center;
      grid-row-start: 2;
    }
    .contact_item {
      text-align: center;
      flex: 0;
    }
    .contact_item  a{
      font-size: 14px;
      font-weight: bold;
      line-height: 140%;
    }
  }
</style>