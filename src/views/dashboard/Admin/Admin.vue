<template>
<div class="dashboard-editor-container">
  <PageTitle title="作品集" />
  <p @click="goPage('/projects/admin')" class="desc">1. 后台管理系统的通用方案</p>
  <p @click="goPage('/projects/im')" class="desc">2. IM抢红包App</p>
</div>
</template>

<script>
import PageTitle from '@pro_common/components/PageTitle/PageTitle.vue'
import router from "@/router/index"
export default {
  name: 'DashboardAdmin',
  methods: {
    goPage(path) { router.push({path}) }
  },
  components: {
    PageTitle
  }
}
</script>

<style lang="scss" scoped>
@import "~@pro_common/styles/colors.scss";
.dashboard-editor-container {
  min-height: 100%;
  padding: 32px 20px;
  /*background-color: rgb(240, 242, 245);*/
  position: relative;
  .desc {
    cursor: pointer;
    font-size: 16px;
    color: $blue-black;
    line-height: 28px;
    margin-bottom: 6px;
  }
}
</style>
