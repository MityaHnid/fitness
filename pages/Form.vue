<template>
  <div>
    <Header />
    <div class="container">
      <div class="form">
        <h2>Send your data</h2>
        <input v-for="placeholderName of placeholderNames" type="text" class="input" v-bind:placeholder="placeholderName" maxlength="38" required>
        <input type="submit" v-on:click="user" class="submit" value="Submit">
      </div>
    </div>
    <Footer />
  </div>

</template>

<style scoped>
.container {
  width: 1240px;
  margin: 0 auto;
}

.form {
  background-image: url("~/static/Subtract (1).png");
  background-size: cover;
  border-radius: 14px;
  margin: 100px auto;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding: 60px 0;
}

.form h2 {
  color: #fff;
  margin-bottom: 17px;
}

.input {
  width: 392px;
  height: 58px;
  padding-left: 30px;
  background: #fff;
  border: 1px solid #C8C2C6;
  border-radius: 38px;
  outline: none;
  margin-bottom: 16px;
  color: #888;
  font-size: 18px;
  font-weight: 400;
  line-height: 28px;
}

.submit {
  width: 392px;
  height: 58px;
  background: #6750A4;
  border: none;
  border-radius: 38px;
  outline: none;
  color: #fff;
  font-size: 18px;
  font-weight: 400;
  line-height: 28px;
  cursor: pointer;
  margin: 8px 0 16px 0;
}

::-webkit-input-placeholder {
  color: #888;
  font-size: 18px;
  font-weight: 400;
  line-height: 28px;
}

@media (max-width: 1320px) {
  .container {
    width: 980px;
  }
  .form {
    margin: 80px auto 50px;
    padding: 0;
  }
}

@media (max-width: 1050px) {
  .container {
    width: 768px;
  }

  .form {
    margin: 50px auto;
  }
}

@media (max-width: 820px){
  .container {
    width: 480px;
  }

  .form {
    margin: 20px auto 50px;
  }
}
</style>

<script>
import Vue from "vue";
export default {
  data: ()=>({
    placeholderNames: ["First Name", "Second Name", "Email", "Adress"]
  }),
    methods: {
      user: function (event) {
        console.log('Привіт! Не виходить витягнути дані з input.value')
      }
    }
}
</script>
