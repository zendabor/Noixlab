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
        <a href="hi@noixlab.com" class="contact_email">hi@noixlab.com</a>
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
        <span class="priv_pol">© 2022 Noixlab. Privacy policy</span>
      </div>
    </div>
  </section>
</template>

<style scoped>
  @media (max-width:420px) {
    .container{
      flex-direction: column;
    }
    .ZigZag,.Reactrangle,.BlueCycle,.BlackCycle {
      display: none;
    }
  }
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
    display: flex;
    align-items: center;
    justify-content: space-evenly;
  }
  .contact_wrap {
    display: flex;
    flex-direction: column;
    gap: 20px;
    text-align: right;
    align-items: flex-end;
  }
  .contact_list {
    display: flex;
    gap: 20px;
    width: 50%;
    flex-wrap: wrap;
    align-items: center;
    justify-content: flex-end;
  }
  .contact_item{
    position: relative;
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
  }
  .contact_email{
    font-size: 40px;
    line-height: 120%;
    position: relative;
  }
  .contact_email:before {
    content: "";
    position: absolute;
    bottom: 0;
    right: 0;
    background: black;
    height: 3px;
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
    width: 56%;
  }
  .img_wrap {
    position: relative;
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
</style>