<template>
  <div class="container">
    <el-card></el-card>
  </div>
</template>

<script>
export default {}
</script>

<style lang='less'>
.container {
  position: absolute;
  width: 100%;
  height: 100%;
  background: url("../../assets/login_bg.jpg") no-repeat center / cover;
  left: 0;
  top: 0;
  .el-card {
    width: 400px;
    height: 350px;
    background-color: #fff;
    position: absolute;
    left: 50%;
    top: 50%;
    transform: translate(-50%, -50%);
  }
}
</style>
