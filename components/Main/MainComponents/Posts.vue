<template>
  <section>
    <div class="container wrapperPosts">
      <div class="wrapperTitleBlock">
        <div class="titleBlock">
          <h2>Our blog posts</h2>
        </div>
      </div>
      <div class="posts">
        <div class="bigPost">
          <a href="#" class="postItem">
            <div class="photoPost">
              <img src="~/static/img_1.png" alt="post">
            </div>
            <div class="postItemContent">
              <p>Return to running after pregnancy – Is your body strong enough for running? </p>
              <div class="timePost">
                <div class="author">
                  <img src="~/static/image author.png" alt="photo author">
                  <span>BY TILDA LOFTIN</span>
                </div>
                <time>JUNE 25, 2021</time>
              </div>
            </div>
          </a>
        </div>
        <div class="wrapperSmallPosts">
          <div class="smallPost">
            <a href="#" class="postItem">
              <div class="photoPost">
                <img src="~/static/img_2.png" alt="post">
              </div>
              <div class="postItemContent">
                <p>Stroller walks</p>
                <div class="timePost">
                  <time>APRIL 21, 2021</time>
                </div>
              </div>
            </a>
          </div>
          <div class="smallPost">
            <a href="#" class="postItem">
              <div class="photoPost">
                <img src="~/static/img_3.png" alt="post">
              </div>
              <div class="postItemContent">
                <p>Playground workout</p>
                <div class="timePost">
                  <time>MARCH 17, 2020</time>
                </div>
              </div>
            </a>
          </div>
          <div class="smallPost">
            <a href="#" class="postItem">
              <div class="photoPost">
                <img src="~/static/img_4.png" alt="post">
              </div>
              <div class="postItemContent">
                <p>Your Essential Fitness Gear for Each Trimester</p>
                <div class="timePost">
                  <time>FEBRUARY 21, 2021</time>
                </div>
              </div>
            </a>
          </div>
          <div class="smallPost">
            <div class="postItem">
              <a href="#" class="photoPost">
                <img src="~/static/img_5.png" alt="post">
              </a>
              <div class="postItemContent">
                <p>What YOU could gain by working with a Woman’s Health Physical Therapist </p>
                <div class="timePost">
                  <time>JANUARY 23, 2020</time>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="paginationPosts">
        <span>Like what you see? View more</span>
        <button>
          <img src="~/static/button_right.png" alt="button">
        </button>
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

.wrapperPosts{
  margin-bottom: 81px;
}

.posts {
  display: flex;
  justify-content: space-between;
  margin-bottom: 32px;
}

.bigPost {
  width: 604px;
  height: 604px;
}

.bigPost p {
  font-size: 32px;
  font-weight: 700;
  line-height: 39px;
  margin-bottom: 12px;
}

.bigPost .photoPost {
  width: 604px;
  height: 604px;
}

.postItem {
  position: relative;
  color: #fff;
}

.bigPost .postItemContent {
  width: 544px;
  position: absolute;
  bottom: 34px;
  left: 32px;
}

.timePost {
  display: flex;
  align-items: center;
  font-size: 16px;
  line-height: 28px;
}

.author {
  display: flex;
  align-items: center;
  margin-right: 35px;
}

.author img {
  margin-right: 9px;
}

.wrapperSmallPosts {
  display: flex;
  flex-wrap: wrap;
  justify-content: right;
  gap: 32px;
}

.smallPost {
  width: 286px;
  height: 286px;
}

.smallPost .postItemContent {
  width: 247px;
  position: absolute;
  bottom: 16px;
  left: 16px;
}

.smallPost p{
  font-size: 24px;
  font-weight: 700;
  line-height: 29px;
  margin-bottom: 6px;
}

.paginationPosts{
  font-size: 24px;
  line-height: 38px;
  color: #23153E;
  display: flex;
  align-items: center;
  justify-content: center;
}

.paginationPosts button{
  border-radius: 50%;
  border: none;
  margin-left: 9px;
  cursor: pointer;
}

@media (max-width: 1320px){
  .wrapperTitleBlock {
    margin-bottom: 64px;
  }

  .bigPost {
    width: 480px;
    height: 480px;
  }

  .bigPost p {
    font-size: 26px;
    line-height: 32px;
    margin-bottom: 15px;
  }

  .bigPost .photoPost {
    width: 480px;
    height: 480px;
  }

  .bigPost .postItemContent {
    width: 450px;
    bottom: 20px;
    left: 20px;
  }

  .wrapperSmallPosts {
    gap: 10px;
  }

  .smallPost {
    width: 235px;
    height: 235px;
  }

  .smallPost .postItemContent {
    width: 210px;
    position: absolute;
    bottom: 12px;
    left: 12px;
  }

  .smallPost p{
    font-size: 21px;
    line-height: 24px;
    margin-bottom: 6px;
  }

  @media (max-width: 1050px){
    .posts {
      flex-direction: column;
      justify-content: center;
      align-items: center;
      gap: 15px;
      margin-bottom: 32px;
    }

    .wrapperSmallPosts {
      width: 480px;
    }

    .smallPost {
      width: 235px;
      height: 235px;
    }
  }
}
</style>
