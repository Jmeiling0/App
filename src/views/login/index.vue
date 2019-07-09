<template>
  <div>
    <van-nav-bar
      title="标题"
/>
  <form>
    <van-cell-group>
  <van-field
    v-model="user.mobile"
    required
    clearable
    label="手机号"
    placeholder="请输入手机号"
  />

  <van-field
    v-model="user.code"
    type="password"
    label="密码"
    placeholder="请输入密码"
    required
  />
    </van-cell-group>
   </form>
   <div>
     <van-button class="login-bt" type="info">登录</van-button>
   </div>
  </div>
</template>

<script>
export default {
  name: 'LoginIndex',
  data () {
    return {
      user: {
        mobile: '',
        code: ''
      }
    }
  }
}
</script>

<style lang="less" scoped>
.login-bt{
  width:100%;
}

</style>
