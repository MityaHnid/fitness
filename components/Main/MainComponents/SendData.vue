<template>
  <section>
    <div class="container">
      <div class="sendData">
        <h2>Send your data</h2>
        <nuxt-link no-prefetch to="/Form">
          <button>
            <a>Go to form</a>
          </button>
        </nuxt-link>
      </div>
    </div>
  </section>
</template>

<style scoped>
.sendData {
  display: flex;
  justify-content: space-around;
  align-items: center;
  background-image: url("~/static/Subtract.png");
  background-size: contain;
  background-repeat: no-repeat;
  color: #fff;
  padding: 100px 0;
  margin-bottom: 160px;
}

.sendData h2 {
  margin-bottom: 0;
}

.sendData button {
  width: 392px;
  height: 58px;
  color: #fff;
  background: #6750A4;
  border-radius: 100px;
  font-size: 18px;
  font-weight: 500;
  line-height: 28px;
  text-align: center;
  border: none;
  cursor: pointer;
}

@media (max-width: 1320px){
  .sendData {
    margin-bottom: 120px;
  }
}

@media (max-width: 1050px){
  .sendData {
    margin-bottom: 90px;
    padding: 60px 0;
  }
}

@media (max-width: 820px){
  .sendData {
    margin-bottom: 60px;
    padding: 22px 0;
  }

  .sendData h2{
    display: none;
  }
}
</style>
