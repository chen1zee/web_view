<template>
<div class="admin-wrap">
  <CardSimple class="card" title="使用到技术栈">
    <div class="flex-wrap">
      <p class="desc back-gray"><span class="red">Vue </span>作为MVVM框架</p>
      <p class="desc back-gray"><span class="red">Vuex </span>全局状态管理</p>
      <p class="desc back-gray"><span class="red">Vue Router </span>路由管理，鉴权拦截</p>
      <p class="desc back-gray"><span class="red">Webpack </span>自动化构建，实现公用资源与业务分离等</p>
      <p class="desc back-gray"><span class="red">NodeJs </span>构建Mock阶段API模拟服务器</p>
    </div>
  </CardSimple>
  <CardSimple class="card" title="项目基本演示">
    <div>
      <video class="video" :src="require('@/assets/demo.mp4')" autoplay="autoplay" loop controls muted />
      <div></div>
    </div>
  </CardSimple>
  <CardSimple class="card" title="项目基本功能点">
    <p class="desc">
      <span class="red">1. </span>页面级，接口级以及按钮级别的权限验证功能
    </p>
    <p class="desc">
      <span class="red">2. </span>动态侧边菜单栏，全屏收缩，快捷导航等实用功能
    </p>
    <p class="desc">
      <span class="red">3. </span>NodeJs编写模拟API服务器，实现文档现行的前端开发流
    </p>
    <p class="desc">
      <span class="red">4. </span>以Model层以及配置文件为中心的CRUD快速成型工具，能实现给定的Model结构，快速生成增删改查页面
    </p>
    <p class="desc">
      <span class="red">5. </span>Webpack构建工具，实现全局公用模块的高度复用，精确打包业务代码
    </p>
  </CardSimple>
</div>
</template>

<script>
import CardSimple from "@pro_common/components/Card/CardSimple";
export default {
  name: "ProjectsAdmin",
  components: {
    CardSimple
  }
}
</script>

<style lang="scss" scoped>
@import "~@pro_common/styles/colors.scss";
.admin-wrap {
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
