<template>
  <section>
    <div class="container instruction">
      <div class="wrapperTitleBlock">
        <div class="titleBlock">
          <h2>How does it work?</h2>
          <p>Easy, fun & essential training for moms</p>
        </div>
      </div>
      <div class="instructionItems">
        <div class="instructionItem">
          <a href="#">
            <img src="~/static/icon.png" alt="icon">
          </a>
          <div>
            <h4>Browse exercises</h4>
            <p>Browse over 100 exercises with a video or picture and a description.</p>
          </div>
        </div>
        <div class="instructionItem">
          <a href="#">
            <img src="~/static/icon (1).png" alt="icon">
          </a>
          <div>
            <h4>Create timeline</h4>
            <p>Take pictures along the way during and after the pregnancy to see the transformation.</p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.instruction {
  margin-bottom: 160px;
}

.wrapperTitleBlock {
  margin-bottom: 84px;
  position: relative;
}

.titleBlock:after {
  content: '';
  position: absolute;
  left: 50%;
  transform: translateX(-50%);
  bottom: -21px;
  width: 46px;
  height: 4px;
  border-bottom: 4px solid #FF2D55;
}

.titleBlock p {
  font-size: 32px;
  font-weight: 500;
  line-height: 39px;
  text-align: center;
}

.instructionItems {
  display: flex;
  justify-content: space-between;
}

.instructionItem {
  width: 610px;
}

.instructionItem{
  display: flex;
}

.instructionItem img {
  margin-right: 20px;
}

@media (max-width: 1320px){
  .instruction {
    margin-bottom: 120px;
  }
}

@media (max-width: 1050px){
  .instruction {
    margin-bottom: 90px;
  }

  .wrapperTitleBlock {
    margin-bottom: 64px;
  }

  .titleBlock p {
    font-size: 26px;
    line-height: 33px;
  }
}

@media (max-width: 820px){
  .instruction {
    margin-bottom: 60px;
  }

  .wrapperTitleBlock {
    margin-bottom: 45px;
  }

  .instructionItem a{
    width: 140px;
  }
}
</style>
