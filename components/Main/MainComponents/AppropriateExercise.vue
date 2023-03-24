<template>
  <section>
    <div class="container wrapperAppropriateExercise">
      <div class="wrapperTitleBlock">
        <div class="titleBlock">
          <h2>Before, during and after pregnancy</h2>
          <p>The app is divided into three different stages to help you choose appropriate exercises. Each
            exercise is carefully selected to ensure safe and appropriate adjustments to follow the pregnancy’s
            progress.</p>
        </div>
      </div>
      <div class="appropriateExercise">
        <article class="appropriateExerciseContent">
          <h3>Before pregnancy</h3>
          <p>Start preparing for pregnancy with safe exercises that build up a strong body.</p>
          <h4>Trimesters</h4>
          <p>The pregnancy is divided into first trimester, second trimester part 1 and 2, and third trimester part 1
            and 2 to provide exercises that are safe for each stage of the pregnancy. Each exercise comes with a video
            and a description so you can safely perform each exercise. Simple put in your due date and you will be
            taken to the proper stage.</p>
        </article>
        <div class="appropriateExerciseImg">
          <img src="~/static/before_img.png" alt="photo exercise">
        </div>
      </div>
      <div class="appropriateExercise duringPregnancy">
        <div class="appropriateExerciseImg">
          <img src="~/static/img_during.png" alt="photo exercise">
        </div>
        <article class="appropriateExerciseContent duringPregnancyContent">
          <h3>During pregnancy</h3>
          <p>Working out during pregnancy has many benefits for both the mom and the baby. It can reduce back pain,
            help prevent gestational diabetes, promote good posture, strength and endurance, and also improve the
            ability to cope with labor.</p>
        </article>
      </div>
      <div class="healthy">
        <img src="~/static/Healthy.png" alt="inscription healthy">
      </div>
    </div>
  </section>
</template>

<style scoped>
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

.wrapperAppropriateExercise {
  position: relative;
  margin-bottom: 160px;
}

.appropriateExercise {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.appropriateExerciseContent {
  width: 562px;
}

.appropriateExerciseContent h3 {
  margin-bottom: 40px;
}

.appropriateExerciseContent h4 {
  margin-top: 16px;
}

.appropriateExerciseImg {
  width: 546px;
  height: 683px;
}

.duringPregnancy {
  margin-top: 68px;
}

.duringPregnancyContent {
  padding-right: 60px;
  margin-right: 40px;
}

.healthy {
  width: 973px;
  height: 218px;
  position: absolute;
  top: 56%;
  right: 0;
  z-index: -1;
}

@media (max-width: 1320px){
  .wrapperAppropriateExercise {
    margin-bottom: 120px;
  }

  .wrapperTitleBlock {
    margin-bottom: 34px;
  }

  .appropriateExerciseContent {
    width: 425px;
  }
  .duringPregnancyContent {
    padding-right: 30px;
    margin-right: -10px;
  }
}

@media (max-width: 1050px){
  .wrapperAppropriateExercise {
    margin-bottom: 60px;
  }

  .titleBlock p {
    font-size: 26px;
    line-height: 33px;
  }

  .appropriateExerciseImg {
    width: 400px;
    height: 560px;
  }

  .appropriateExerciseContent {
    width: 350px;
  }

  .healthy {
    width: 760px;
    height: 180px;
    position: absolute;
    top: 54%;
  }

  .duringPregnancy {
    margin-top: 45px;
  }
}

@media (max-width: 820px){
  .appropriateExercise {
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-direction: column;
  }

  .healthy {
    width: 475px;
    height: 120px;
    position: absolute;
    top: 58%;
  }

}
</style>
