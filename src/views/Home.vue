<script setup>
const realizes = [
  {
    name: '二三维一体场景可视化',
    desc: '',
    pic: 'https://dc.dvgis.cn/examples/previews/mini-scene/dfmz.gif'
  },
  {
    name: '知名地图厂商的地图接入',
    desc: '',
    pic: ''
  },
  {
    name: '',
    desc: '',
    pic: ''
  },
  {
    name: '',
    desc: '',
    pic: ''
  },
  {
    name: '',
    desc: '',
    pic: ''
  },
  {
    name: '',
    desc: '',
    pic: ''
  }
]
</script>

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
    <div class="realize">
      <div class="title">
        <div class="bg">平台可以实现</div>
        <div class="name">平台可以实现</div>
      </div>
      <div class="desc">
        <div
          class="item"
          v-for="(item, index) in realizes"
          :key="'realize' + index"
        >
          <div class="index">0{{ index + 1 }}</div>
          {{ item.name }}
          {{ item.desc }}
          <img class="img" :src="item.pic" />
        </div>
      </div>
    </div>
    <div class="feature">
      <div class="title">
        <div class="bg">平台的优势</div>
        <div class="name">平台的优势</div>
      </div>
    </div>
    <div class="why">
      <div class="title">
        <div class="bg">为什么选择</div>
        <div class="name">为什么选择</div>
      </div>
    </div>
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
  .realize,
  .feature,
  .why {
    height: 100vh;
    padding: 2rem 6rem;
    .title {
      width: 100%;
      text-align: center;
      .bg {
        color: rgba(0, 0, 0, 0.05);
        font-size: 3.5rem;
        font-weight: 700;
      }
      .name {
        font-size: 2.5rem;
        font-weight: 700;
        transform: translate(0, -3rem);
      }
    }
  }

  .realize {
    .desc {
      display: grid;
      grid-template-columns: repeat(3, 33.33%);
      .item {
        height: 30vh;
        border: 0.5px solid #cecece;
        position: relative;
        padding: 3rem 2rem;
        .index {
          color: #cc1517;
          font-size: 2rem;
          margin-bottom: 3rem;
        }
        img {
          border-radius: 50%;
          position: absolute;
          top: 0.5rem;
          right: 0.5rem;
          scale: 0.9;
        }
      }
    }
  }
}
</style>
