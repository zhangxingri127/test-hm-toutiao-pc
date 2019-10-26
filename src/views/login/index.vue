<template>
  <div class="container">
    <el-card>
      <img src="../../assets/logo_index.png" alt />
      <el-form :model="LoginForm">
        <el-form-item>
          <el-input v-model="LoginForm.name"></el-input>
        </el-form-item>
        <el-form-item>
          <el-input v-model="LoginForm.name" style="width:240px;margin-right:8px"></el-input>
          <el-button>发送验证码</el-button>
        </el-form-item>
        <el-checkbox :value="true">我已阅读并同意用户协议和隐私条款</el-checkbox>
        <el-form-item>
          <el-button type="primary" style="width:100%;margin-top:35px">立即创建</el-button>
        </el-form-item>
      </el-form>
    </el-card>
  </div>
</template>

<script>
export default {
  data () {
    return {
      checked: '',
      LoginForm: { name: '' }
    }
  }
}
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
    img {
      width: 200px;
      margin: 0 auto 20px;
      display: block;
    }
  }
}
</style>
