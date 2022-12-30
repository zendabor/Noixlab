<script>
export default {
  name: "TrustedCompany"
}
</script>
<template>
  <section>
    <h3 class="TrustedCompany_title">We are Trusted</h3>
    <ul class="TrustedCompany_list">
      <li class="TrustedCompany_item">
        <div class="img_wrap">
          <img src="/src/assets/img/mobility01.png" alt="">
        </div>
      </li>
      <li class="TrustedCompany_item">
        <div class="img_wrap">
          <img src="/src/assets/img/mobility02.png" alt="">
        </div>
      </li>
      <li class="TrustedCompany_item">
        <div class="img_wrap">
          <img src="/src/assets/img/mobility03.png" alt="">
        </div>
      </li>
      <li class="TrustedCompany_item">
        <div class="img_wrap">
          <img src="/src/assets/img/mobility04.png" alt="">
        </div>
      </li>
      <li class="TrustedCompany_item">
        <div class="img_wrap">
          <img src="/src/assets/img/mobility05.png" alt="">
        </div>
      </li>
      <li class="TrustedCompany_item">
        <div class="img_wrap">
          <img src="/src/assets/img/mobility06.png" alt="">
        </div>
      </li>
      <li class="TrustedCompany_item">
        <div class="img_wrap">
          <img src="/src/assets/img/mobility07.png" alt="">
        </div>
      </li>
      <li class="TrustedCompany_item">
        <div class="img_wrap">
          <img src="/src/assets/img/mobility08.png" alt="">
        </div>
      </li>
      <li class="TrustedCompany_item">
        <div class="img_wrap">
          <img src="/src/assets/img/mobility09.png" alt="">
        </div>
      </li>
      <li class="TrustedCompany_item">
        <div class="img_wrap">
          <img src="/src/assets/img/mobility010.png" alt="">
        </div>
      </li>
      <li class="TrustedCompany_item">
        <div class="img_wrap">
          <img src="/src/assets/img/mobility011.png" alt="">
        </div>
      </li>
      <li class="TrustedCompany_item">
        <div class="img_wrap">
          <img src="/src/assets/img/mobility012.png" alt="">
        </div>
      </li>
      <li class="TrustedCompany_item">
        <div class="img_wrap">
          <img src="/src/assets/img/mobility013.png" alt="">
        </div>
      </li>
    </ul>
    <span class="line"></span>
  </section>
</template>

<style scoped>
section {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-around;
}
.TrustedCompany_title {
  font-size: 40px;
  line-height: 140%;
  color: #283534;
}
.TrustedCompany_list {
  display: flex;
  flex-wrap: wrap;
  width: 59%;
  gap: 65px 75px;
  justify-content: space-evenly;
  margin-bottom: 70px;
}
.TrustedCompany_item {
  display: flex;
  align-items: center;
  justify-content: center;
}
.line {
  height: 2px;
  background-color: black;
  width: 35%;
}
@media (max-width: 420px) {
  section {
    padding: 48px 0 25px;
  }
  .TrustedCompany_list {
    gap: 25px 75px;
    justify-content: space-between;
    align-items: center;
    width: 100%;
    padding: 0 30px;
    margin-bottom: 50px;
  }
  .TrustedCompany_title {
    margin-bottom: 25px;
  }
  .TrustedCompany_item {
    width: 38%;
  }
  .TrustedCompany_item:last-child{
    flex: 1;
  }
  .line {
    width: 70%;
  }
}
</style>

