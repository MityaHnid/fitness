<template>
  <section>
    <div class="container banner">
      <div class="bannerContent">
        <h1>Strong for life with us </h1>
        <p>
          The best Pre/postnatal fitness app! 100 exercises divided in before, during and after pregnancy. Stay strong
          and healthy through all stages of pregnancy.
        </p>
        <div class="wrapperMobileApp">
          <div class="mobileApp">
            <a href="#">
              <img src="~/static/Mobile app store badge.png" alt="icon App Store">
            </a>
          </div>
          <div class="mobileApp">
            <a href="#">
              <img src="~/static/Mobile app googlePlay.png" alt="icon GooglePlay">
            </a>
          </div>
        </div>
      </div>
      <div class="bannerImage"></div>
    </div>
  </section>
</template>

<style scoped>
section {
  margin-bottom: 154px;
}

.banner {
  position: relative;
  background-image: url("~/static/bannerBg.png");
  background-size: contain;
  background-repeat: no-repeat;
  width: 100%;
  height: 770px;
  display: flex;
  justify-content: space-between;
}

.bannerContent {
  width: 498px;
  margin: 107px 0 0 105px;
}

.bannerContent p {
  font-size: 24px;
  line-height: 38px;
  margin: 70px 0 37px;
}

.wrapperMobileApp {
  display: flex;
}

.mobileApp {
  width: 170px;
  height: 50px;
  margin-right: 40px;
}

.bannerImage {
  position: absolute;
  right: 0;
  top: 20px;
  width: 637px;
  height: 860px;
  background-image: url("~/static/BannerImg.png");
  background-size: cover;
}

@media (max-width: 1320px) {
  section {
    margin-bottom: 120px;
  }

  .banner {
    height: 620px;
  }

  .bannerContent {
    margin: 75px 0 0 105px;
  }

  .bannerImage {
    top: 0;
    width: 515px;
    height: 715px;
  }
}

@media (max-width: 1050px){
  section {
    margin-bottom: 90px;
  }

  .banner {
    height: 480px;
  }

  .bannerContent {
    width: 360px;
    margin: 50px 0 0 40px;
  }

  .bannerContent p {
    font-size: 18px;
    line-height: 32px;
    margin: 40px 0 12px;
  }

  .bannerImage {
    width: 410px;
    height: 560px;
  }
}

@media (max-width: 820px){
  section {
    margin-bottom: 50px;
  }

  .banner {
    height: 300px;
  }

  .bannerImage {
    display: none;
  }

  .bannerContent {
    width: 440px;
    margin: 15px 0 0 15px;
  }

  .bannerContent p {
    font-size: 18px;
    line-height: 26px;
    margin: 30px 0 12px;
  }

  .mobileApp {
    width: 145px;
    height: 38px;
    margin-right: 35px;
  }
}
</style>
