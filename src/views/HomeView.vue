<template>
  <div class="container">
    <div class="row">
      <div class="col-md-6">
        <!-- 轮播 -->
        <div id="carouselExampleCaptions" class="carousel slide" data-bs-ride="carousel">
          <div class="carousel-indicators">
            <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="0" class="active"
              aria-current="true" aria-label="Slide 1"></button>
            <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="1"
              aria-label="Slide 2"></button>
            <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="2"
              aria-label="Slide 3"></button>
          </div>
          <div class="carousel-inner imgboder">
            <div class="carousel-item active">
              <img src="https://img.zimei.xyz/202207041928071.png" class="d-block w-100" alt="图片挂掉了(ಥ _ ಥ)">
              <div class="carousel-caption d-none d-md-block">
                <h5>First slide label</h5>
                <p>Some representative placeholder content for the first slide.</p>
              </div>
            </div>
            <div class="carousel-item">
              <img src="http://img.zimei.xyz/202201272327591.jpg" class="d-block w-100" alt="图片挂掉了(ಥ _ ಥ)">
              <div class="carousel-caption d-none d-md-block">
                <h5>Second slide label</h5>
                <p>Some representative placeholder content for the second slide.</p>
              </div>
            </div>
            <div class="carousel-item">
              <img src="http://img.zimei.xyz/202201282308685.jpeg" class="d-block w-100" alt="图片挂掉了(ಥ _ ಥ)">
              <div class="carousel-caption d-none d-md-block">
                <h5>Third slide label</h5>
                <p>Some representative placeholder content for the third slide.</p>
              </div>
            </div>
          </div>
          <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleCaptions"
            data-bs-slide="prev">
            <span class="carousel-control-prev-icon" aria-hidden="true"></span>
            <span class="visually-hidden">Previous</span>
          </button>
          <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleCaptions"
            data-bs-slide="next">
            <span class="carousel-control-next-icon" aria-hidden="true"></span>
            <span class="visually-hidden">Next</span>
          </button>
        </div>

      </div>
      <div class="col-md-6">
        <!-- 公告card -->
        <div class="card shadow-sm ">
          <div class="card-body">
            <h5 class="card-title">公告</h5>
            <h6 class="card-subtitle mb-2 text-muted">note</h6>
            <p><a class="card-link"
                href="https://www.botzone.org.cn/static/gamecontest2021s.html">点击进入</a>第十三届北京大学游戏对抗赛主页</p>
            <p>
              欲查规则？点击
              <a href="#" class="card-link">游戏规则</a>
              进入游戏一览。
            </p>
            <p>
              参加比赛？点击
              <a href="#" class="card-link">比赛</a>
              进入小组一览。
            </p>
            <p>
              提交程序？点击
              <a href="#" class="card-link">程序</a>
              或顶栏按钮管理你的 Bot。
            </p>
          </div>
        </div>

      </div>
    </div>
  </div>
  <ContentBase>
    <div>

      <div class="alert alert-success">
        <strong>Welcome</strong> 导航
      </div>

      <br>
      <p>欢迎来到本网站，你可以将这里当作你的网上空间</p>
      <p>这里的人说话好听，超级有趣的偶</p>
      <p>这么说你很勇喽</p>
      <p>是的啊</p>
      <p>欢迎来到本网站，你可以将这里当作你的网上空间</p>
      <p>这里的人说话好听，超级有趣的偶</p>
      <p>这么说你很勇喽</p>
      <p>是的啊</p>
      <p>欢迎来到本网站，你可以将这里当作你的网上空间</p>
      <p>这里的人说话好听，超级有趣的偶</p>
      <p>这么说你很勇喽</p>
      <p>是的啊</p>
      <p>
        <a href="https://www.zimei.xyz/" target="_blank">
          <img src="http://img.zimei.xyz/202201282100719.gif" width="" />
        </a>
      </p>
    </div>
  </ContentBase>
</template>

<script>
import ContentBase from '../components/ContentBase';

export default {
  name: 'HomeView',
  components: {
    ContentBase,
  }
}
</script>

<style scoped>
/* 轮播 */
.container {
  margin-top: 20px;
}

/* 超链接 */
ul {
  list-style-type: none;
  /*清楚项目符号*/
}

a:hover {
  color: rgb(89, 192, 127);
  background: transparent;
}

a {
  /*完全清除超链接下划线效果*/
  text-decoration: none;
}

/* 轮播圆角 */
.imgboder{
  border-radius: 0.5rem;
}

</style>
