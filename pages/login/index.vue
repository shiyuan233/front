<template>
  <div class="login-box">
    <el-form :mode="form">
      <el-form-item label="用户名" prop="userName">
        <el-input v-model="form.userName"></el-input>
      </el-form-item>
      <el-form-item label="密码" prop="password">
        <el-input type="password" v-model="form.password"></el-input>
      </el-form-item>
    </el-form>
  </div>
</template>

<script>
export default {
  data() {
    return {
      form: {
        userName: "admin",
        password: "",
      },
    };
  },
};
</script>

<style lang="stylus" scoped>
.login-box
  width: 800px
  margin: 0 auto
</style>
