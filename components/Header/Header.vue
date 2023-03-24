<template>
  <div class="container header">
    <nuxt-link class="logo" to="/">
      <a>LOGO</a>
    </nuxt-link>
    <div class="headerContent">
      <nav>
        <ul>
          <li v-for="navItem of navItems" :key="navItem">
            <a href="#">{{navItem}}</a>
          </li>
        </ul>
      </nav>
      <div class="wrapperDownload">
        <button class="button">Download</button>
        <div class="subMenu downloadMenu">
          <ul>
            <li><a href="#">App Store</a></li>
            <li><a href="#">Google Play</a></li>
          </ul>
        </div>
      </div>
      <div class="wrapperLanguage">
        <div class="language">
          <span>Eng</span>
        </div>
        <div class="subMenu languageMenu">
          <ul>
            <li class="downloadMenuItem">
              <a href="#">
                <img src="~/static/Sverige.png" alt="icon language">
                <span>Sverige</span>
              </a>
            </li>
            <li class="downloadMenuItem">
              <a href="#">
                <img src="~/static/English.png" alt="icon language">
                <span>English</span>
              </a>
            </li>
          </ul>
        </div>
      </div>
    </div>
    <div class="burger">
      <span></span>
    </div>
  </div>
</template>

<style scoped>
a {
  color: #23153E;
}

nav ul {
  display: flex;
  align-items: center;

}

nav ul li {
  margin: 0 12px;
  color: #23153E;
}

.container {
  width: 1240px;
  margin: 0 auto;
}

.button {
  font-size: 18px;
  font-weight: 500;
  line-height: 20px;
  letter-spacing: 0.1px;
  padding: 12px 55px;
  background: #6750A4;
  border-radius: 100px;
  border: none;
  color: #fff;
}

.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 86px;
}

.logo {
  font-size: 40px;
  font-weight: 700;
  line-height: 49px;
  color: #6750A4;
  margin: 28px 0 23px;
}

.headerContent {
  display: flex;
  color: #23153E;
}

.language{
  cursor: pointer;
  padding-right: 15px;
}

.language:after {
  content: '';
  width: 8px;
  height: 8px;
  position: absolute;
  top: 8px;
  right: 0;
  border: solid #6750A4;
  border-width: 0 2px 2px 0;
  transform: rotate(45deg);
}

.wrapperDownload {
  position: relative;
  margin: 0 21px 0 26px;
}

.downloadMenu {
  width: 100%;
  padding: 7px 12px;
}

.wrapperLanguage {
  position: relative;
}

.languageMenu {
  width: 145px;
}

.downloadMenuItem a{
  display: flex;
}

.subMenu {
  position: absolute;
  height: 70px;
  top: 55px;
  box-shadow: 0 4px 4px 0 #00000040;
  border-radius: 4px;
  font-size: 14px;
  line-height: 28px;
}

.burger{
  width: 46px;
  height: 46px;
  cursor: pointer;
  display: none;
}
.burger > span,
.burger > span:before,
.burger > span:after{
  display: block;
  position: absolute;
  width: 46px;
  height: 3px;
  background: #23153E;
}
.burger > span:before{
  content: '';
  top: -12px;
}
.burger > span:after{
  content: '';
  top: 12px;
}

@media (max-width: 1500px) {
  .headerContent {
    padding-right: 95px;
  }
}

@media (max-width: 1320px) {
  .container {
    width: 980px;
  }

  nav ul li {
    margin: 0 7px;
  }
}

@media (max-width: 1050px) {
  .container {
    width: 768px;
  }

  .header {
    margin-bottom: 10px;
  }

  .headerContent{
    display: none;
  }

  .burger{
    display: flex;
    align-items: center;
    margin: 8px 0;
  }
}

@media (max-width: 820px){
  .container {
    width: 480px;
  }
}
</style>

<script>
export default {
  data: ()=>({
    navItems: ["Home", "About", "Pricing", "Facts", "Blog", "Support"]
  })
}
</script>
