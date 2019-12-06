<template>
<div class="admin-wrap">
  <CardSimple class="card" title="使用到技术栈">
    <div class="wrap">
      <p class="desc"><span class="red">Vue </span>作为MVVM框架</p>
      <p class="desc"><span class="red">Vuex </span>全局状态管理</p>
      <p class="desc"><span class="red">Vue Router </span>路由管理，鉴权拦截</p>
      <p class="desc"><span class="red">Webpack </span>自动化构建，实现公用资源与业务分离等</p>
      <p class="desc"><span class="red">NodeJs </span>构建Mock阶段API模拟服务器</p>
    </div>
  </CardSimple>
  <CardSimple class="card" title="项目基本演示">
    <div>
      <video class="video" :src="require('@/assets/demo.mp4')" autoplay="autoplay" loop controls muted />
      <div></div>
    </div>
  </CardSimple>
  <CardSimple class="card" title="项目基本功能">
    <div class="wrap">
      <p class="desc"><span class="red"></span></p>
    </div>
  </CardSimple>
</div>
</template>

<script>
import CardSimple from "@pro_common/components/Card/CardSimple";
export default {
  name: "Admin",
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
  .wrap {
    display: flex;
    flex-wrap: wrap;
  }
  .desc {
    font-size: 18px;
    line-height: 38px;
    color: $level-2-word;
    margin: 0 20px;
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
