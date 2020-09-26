<template>
  <div class="login_container">
    <Card class="login_box">
        <!-- 登录 slot改变位置 -->
        <p slot="title">
            <Icon type="ios-finger-print"></Icon>
            SiFou-foot-Web
        </p>
        <!-- 注册 -->
        <!-- <a href="#" slot="extra" @click.prevent="">
            Sign up
        </a> -->
        <!-- 账号密码 -->
        <Form ref="formInline" :model="formInline" :rules="ruleInline">
          <FormItem prop="user">
              <Input type="text" v-model="formInline.user" placeholder="账号/邮箱/手机号" clearable>
                  <Icon type="ios-person-outline" slot="prepend"></Icon>
              </Input>
          </FormItem>
          <FormItem prop="password">
              <Input type="password" v-model="formInline.password" placeholder="请输入密码" clearable>
                  <Icon type="ios-lock-outline" slot="prepend"></Icon>
              </Input>
          </FormItem>
          <FormItem>
              <Button type="primary" @click="handleSubmit('formInline')">登录</Button>
              <Button type="dashed" @click="resetLoginForm()" style="transform: translate(10px, 0);" >重置</Button>
          </FormItem>
        </Form>
    </Card>
  </div>
</template>

<script>
import {loginvueSubmit} from '../api/Login.js'

export default {
  name: 'Login',
  data () {
    return {
      formInline: {
          user: '',
          password: ''
      },
      // 预验证规则
      ruleInline: {
          user: [{ required: true, message: 'Please fill in the user name', trigger: 'blur' }],
          password: [{ required: true, message: 'Please fill in the password.', trigger: 'blur' },
                     { type: 'string', min: 6, message: 'The password length cannot be less than 6 bits', trigger: 'blur' }]
      }
    } 
  },
  methods: {
    //提交登录
    handleSubmit(name) {
        this.$refs[name].validate((valid) => {
            if (valid) {
              this.$Message.success('Success!');
            } else {
              this.$Message.error('Fail!');
            }
        })
    },
    //重置信息
    resetLoginForm(){
        this.$refs.formInline.resetFields();
    }

  }
}
</script>

<style lang="less" scoped>
  .login_container{
      background-color: rgb(200, 200, 200);
      height: 100%;
      .login_box{
      width: 450px;
      height: 300px;
      background-color: #fff;
      position: absolute;
      left: 50%;
      top: 50%;
      transform: translate(-50%, -50%);
      }
  }
</style>