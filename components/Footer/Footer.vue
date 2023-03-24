<template>
  <div class="footer">
    <div class="container">
      <nuxt-link class="logo" to="/">
        <a>LOGO</a>
      </nuxt-link>
      <nav>
        <ul>
          <li v-for="navItemFirst of navItemsFirst" :key="navItemFirst"><a href="#">{{ navItemFirst }}</a></li>
        </ul>
      </nav>
      <nav>
        <ul>
          <li v-for="navItemSecond of navItemsSecond" :key="navItemSecond"><a href="#">{{ navItemSecond }}</a></li>
        </ul>
      </nav>
      <div class="socialNetwork">
        <ul>
          <li>
            <a href="#">
              <img src="~/static/Facebook.png" alt="icon Facebook">
            </a>
          </li>
          <li>
            <a href="#">
              <img src="~/static/Instagram.png" alt="icon Instagram">
            </a>
          </li>
          <li>
            <a href="#">
              <img src="~/static/YouTube.png" alt="icon YouTube">
            </a>
          </li>
          <li>
            <a href="#">
              <img src="~/static/Pinterest.png" alt="icon Pinterest">
            </a>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<style scoped>
a {
  color: #fff;
}

nav {
  width: 286px;
  margin-right: 36px;
}

.footer {
  background: #423C4E;
  padding: 74px 0 78px;
  color: #fff;
}

.container {
  width: 1240px;
  margin: 0 auto;
}

.footer .container {
  display: flex;
  align-items: center;
}

.logo {
  margin-right: 92px;
}

.logo a {
  font-size: 40px;
  font-weight: 700;
  line-height: 49px;
}

.socialNetwork ul {
  display: flex;
  align-items: center;
}

.socialNetwork ul li {
  margin-right: 20px;
}

@media (max-width: 1320px) {
  .container {
    width: 980px;
  }
}

@media (max-width: 1050px) {
  .footer {
    padding: 45px 0 50px;
  }

  .container {
    width: 768px;
  }

  .logo {
    margin-right: 60px;
  }

  nav {
    width: 160px;
    margin-right: 30px;
  }
}

@media (max-width: 820px) {
  .footer {
    padding: 25px 0 30px;
  }

  nav {
    display: none;
  }

  .container {
    width: 480px;
  }

  .socialNetwork ul li {
    margin: 7px 20px 0 0;
  }
}
</style>

<script>
export default {
  data: () => ({
    navItemsFirst: ["About Us", "Blog", "Support"],
    navItemsSecond: ["Terms & Conditions", "Privacy Policy", "Cookies"]
  })
}
</script>
