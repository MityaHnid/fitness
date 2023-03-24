<template>
  <div>
    <Header />
    <Main/>
    <Footer />
  </div>
</template>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

@font-face {
  font-family: Montserrat;
  src: url("~/static/fonts/Montserrat-VariableFont_wght.ttf");
}

html {
  height: 100%;
}

body {
  height: 100%;
  display: flex;
  flex-direction: column;
  margin: 0 auto;
  background: #fff;
  font-family: Montserrat, sans-serif;
  font-size: 18px;
  line-height: 28px;
  color: #443A5A;
}

img {
  max-width: 100%;
}

a{
  text-decoration: none;
  cursor: pointer;
}

li{
  list-style-type: none;
}

button{
  cursor: pointer;
}

h1{
  font-size: 56px;
  font-weight: 700;
  line-height: 68px;
  color: #23153E;
  position: relative;
}

h2{
  font-size: 50px;
  font-weight: 700;
  line-height: 61px;
  text-align: center;
  margin-bottom: 24px;
}

h3{
  font-size: 40px;
  font-weight: 700;
  line-height: 49px;
  position: relative;
}

h4{
  font-size: 32px;
  font-weight: 500;
  line-height: 39px;
}

h1:after,
h3:after{
  content: '';
  position: absolute;
  bottom: -21px;
  left: 0;
  width: 46px;
  height: 4px;
  border-bottom: 4px solid #FF2D55;
}

@media (max-width: 1050px){
  body {
    font-size: 16px;
    line-height: 26px;
  }

  h1{
    font-size: 46px;
    line-height: 58px;
  }

  h2{
    font-size: 40px;
    line-height: 51px;
    margin-bottom: 16px;
  }

  h3{
    font-size: 34px;
    line-height: 43px;
  }

  h4{
    font-size: 28px;
    line-height: 35px;
  }
}

@media (max-width: 820px){
  h1{
    font-size: 38px;
    line-height: 44px;
  }

  h1:after,
  h3:after{
    content: '';
    position: absolute;
    bottom: -15px;
    left: 0;
    width: 40px;
    height: 4px;
    border-bottom: 4px solid #FF2D55;
  }

  h2{
    font-size: 34px;
    line-height: 40px;
    margin-bottom: 12px;
  }

  h3{
    font-size: 28px;
    line-height: 36px;
  }

  h4{
    font-size: 24px;
    line-height: 30px;
  }
}
</style>

<script>
export default {
  name: 'IndexPage'
}
</script>
