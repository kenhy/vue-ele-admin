<template>
<div class='error-page'>
  <div class="error-code">40<span>3</span></div>
  <div class="error-desc">你没有权限访问该页面哦</div>
  <div class="error-handle">
      <router-link to="/">
        <el-button type="primary">返回首页</el-button>
      </router-link>
      <el-button class="error-btn" @click="goBack">返回上一页</el-button>
  </div>
</div>
</template>

<script>
export default {
  components: {},
  methods: {
    goBack () {
      this.$router.go(-1)
    }
  }
}
</script>

<style scoped>
@import url('../assets/css/error.css');
</style>
