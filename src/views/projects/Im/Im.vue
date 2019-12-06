<template>
<div class="wrap">
  <CardSimple class="card" title="使用到技术栈">
    <div class="flex-wrap">
      <p class="desc back-gray"><span class="red">React </span>作为MVVM框架</p>
      <p class="desc back-gray"><span class="red">Typescript </span>Javascript的超集，提供强类型支持</p>
      <p class="desc back-gray"><span class="red">Mobx </span>Model层管理，让react的视图更新更智能</p>
      <p class="desc back-gray"><span class="red">Android </span>安卓原生代码供ReactNative使用</p>
      <p class="desc back-gray"><span class="red">WebSocket </span> 原生Websocket封装订阅发布模式，并实现心跳，重连等逻辑</p>
    </div>
  </CardSimple>
  <CardSimple class="card" title="项目基本演示">
    <div>
      <video class="video" :src="require('@/assets/demo_phone.mp4')" autoplay="autoplay" loop controls muted />
    </div>
  </CardSimple>
  <CardSimple class="card" title="项目基本功能点">
    <p class="desc">
      <span class="red">1. </span>React MVVM框架，使用React hook 开发Model层与视图分离，高复用的组件
    </p>
    <p class="desc">
      <span class="red">2. </span>ReactNavigation 作为路由管理器
    </p>
    <p class="desc">
      <span class="red">3. </span>Mobx状态管理，监听数据层的变化，达到精准按需重渲染视图
    </p>
    <p class="desc">
      <span class="red">4. </span>极光推送等第三方Android API的对接使用
    </p>
    <p class="desc">
      <span class="red">5. </span>手机端数据库表设计（如聊天记录，通讯录存储等）
    </p>
  </CardSimple>
</div>
</template>

<script>
import CardSimple from "@pro_common/components/Card/CardSimple";

export default {
  name: "ProjectsIm",
  components: {
    CardSimple
  }
}
</script>

<style lang="scss" scoped>
@import "~@pro_common/styles/colors.scss";
.wrap {
  padding: 20px;
  .card {
    margin-bottom: 30px;
  }
  .flex-wrap {
    display: flex;
    flex-wrap: wrap;
  }
  .desc {
    font-size: 16px;
    line-height: 38px;
    color: $level-2-word;
    margin: 0 20px;
  }
  .back-gray {
    background-color: $gray-less;
    padding: 10px;
    line-height: 28px;
    border-radius: 5px;
    margin-bottom: 10px;
  }
  .video {
    width: 600px;
    height: 400px;
  }
  /** 公共 */
  .red {
    color: $red;
  }
}

</style>
