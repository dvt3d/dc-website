<script setup></script>

<template>
  <div class="home">
    <div class="banner">
      <div class="desc">
        <span>一款快速构建三维地理视化应用的开源开发平台</span>
      </div>
      <div class="pic">
        <img src="/assets/images/earth.gif" />
      </div>
    </div>
    <div class="realize"></div>
    <div class="feature"></div>
  </div>
</template>

<style lang="scss" scoped>
.home {
  width: 100%;
  height: 100%;
  .banner {
    width: 100%;
    height: 100vh;
    background: #1c1c1c;
    display: flex;
    align-items: center;
    justify-content: space-around;
    color: #fff;
    .desc {
      span {
        font-size: 2.5rem;
      }
    }
    .pic {
      img {
        width: 500px;
        height: 500px;
      }
    }
  }
  .realize {
    height: 100vh;
  }
  .feature {
    height: 100vh;
  }
}
</style>
