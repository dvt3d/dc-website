<script setup>
const realizes = [
  {
    name: '二三维一体场景可视化',
    desc: '二三维无缝切换，一套代码兼容多种风格。借助该框架，可轻松将地图、各类矢量数据及模型融入场景，让场景呈现更贴近真实世界的视觉效果',
    pic: '/examples/previews/mini-scene/dfmz.gif'
  },
  {
    name: '知名地图厂商的地图接入',
    desc: '高德、百度、腾讯、天地图、Google、MapBox等主流地图厂商的无缝接入，针对国内地图数据，可灵活进行偏移处理',
    pic: 'examples/previews/mini-scene/ljz.gif'
  },
  {
    name: '数据的统一管理，并支持动画与特效',
    desc: '通过图层管理操作，可对数据进行针对性筛选与整体控制，支持线、面、圆、模型等的材质效果及细节动画，实现数据属性随时间变化',
    pic: 'examples/previews/overlay/dynamic_model.gif'
  },
  {
    name: '相机的路径漫游与定点巡航',
    desc: '相机的自动漫游与巡航功能，可根据预设路线运行，便于快速定位并查看重点区域',
    pic: 'examples/previews/animation/flying.gif'
  },
  {
    name: '三维空间分析',
    desc: '强大的测距、面积、高度等量算工具，并支持可视域、通视分析以及日照模拟等三维场景智能分析功能，能够充分满足多样化需求',
    pic: 'examples/previews/mini-scene/factory.gif'
  },
  {
    name: '第三方图形库的融合',
    desc: 'Turf、Heatmap、Echarts等多种第三方可视化库的融合，降低用户学习成本，减少重复投入，提升开发效率，助力高效可视化应用开发',
    pic: 'examples/previews/datav/migrate.gif'
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
          <h3>{{ item.name }}</h3>
          <p>{{ item.desc }}</p>
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
    margin-bottom: 2rem;
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
    padding: 2rem 8rem;
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
        h3 {
          width: 14vw;
          height: 12vh;
        }
        p {
          color: #8f8f8f;
          text-align: justify;
        }
        .img {
          border-radius: 10%;
          position: absolute;
          top: 1rem;
          right: 1rem;
          scale: 0.9;
        }
      }
    }
  }
}
</style>
