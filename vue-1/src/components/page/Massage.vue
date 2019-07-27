<template>
  <div class="container">
    <h3>个人信息</h3>
    <el-row>
      <el-col :span="3">
        <div class="user-avator">
          <img src="../../assets/img/img.jpg" />
        </div>
      </el-col>
      <el-col :span="3">
        <p>昵称：{{name}}</p>
      </el-col>
      <el-col :span="3">
        <p>身份：{{role}}</p>
      </el-col>
      <el-col :span="3">
        <p>手机号：173xxxx3230{{number}}</p>
      </el-col>
    </el-row>
    <h3>安全设置</h3>
    <el-row>
      <el-col :span="2">修改密码</el-col>
      <el-col :span="4">
        <el-input placeholder="请输入手机号" v-model="input0"></el-input>
      </el-col>
    </el-row>
    <el-row>
      <el-col :span="2">验证码</el-col>
      <el-col :span="4">
        <el-input placeholder="请输入验证码" v-model="input1"></el-input>
      </el-col>
      <el-col :span="2">
        <a class="verify" href="#">获取验证码</a>
      </el-col>
    </el-row>
    <el-row>
      <el-col :span="2">修改密码</el-col>
      <el-col :span="4">
        <el-input placeholder="请输入手机号" v-model="input2"></el-input>
      </el-col>
    </el-row>
    <h3>更换手机号</h3>
    <el-row>
      <el-col :span="2">新号码</el-col>
      <el-col :span="4">
        <el-input placeholder="请输入新手机号" v-model="input3"></el-input>
      </el-col>
    </el-row>
    <el-row>
      <el-col :span="2">验证码</el-col>
      <el-col :span="4">
        <el-input placeholder="请输入验证码" v-model="input4"></el-input>
      </el-col>
      <el-col :span="2">
        <a class="verify" href="#">获取验证码</a>
      </el-col>
    </el-row>
    <el-row>
      <el-col :span="2" :offset="5">
        <el-button type="primary">更换</el-button>
      </el-col>
    </el-row>
    <div class="text">
      <h3>还原设置</h3>
      <p>
        <a href="#">还原所有设置</a>
      </p>
      <p>抹掉所有内容和设置</p>
      <h3>检查更新</h3>
      <p>当前版本1.01.1【升级】</p>
      <h3>备份</h3>
      <p>一键备份与恢复</p>
    </div>
  </div>
</template>
<script>
export default {
    data() {
    return {
      input0: '',
      input1: '',
      input2: '',
      input3: '',
      input4: '',
    }
  }
};
</script>
<style scoped>
.container {
  padding: 30px;
  background: #fff;
  border: 1px solid #ddd;
  border-radius: 5px;
}
.user-avator {
  margin-left: 20px;
}
.user-avator img {
  display: block;
  width: 60px;
  height: 60px;
  border-radius: 50%;
}
h3 {
  margin-bottom: 20px;
}
h3:nth-of-type(2),
h3:nth-of-type(3) {
  margin-top: 30px;
}
.el-row:nth-of-type(1) {
  margin-left: 0;
}
.el-row {
  line-height: 50px !important;
  margin-left: 15px;
}
.el-row .el-col p {
  border: #dddddd 1px solid;
  border-radius: 5px;
  height: 30px;
  width: 110px;
  line-height: 30px;
  text-align: center;
  margin-top: 10px;
}
.el-row .el-col:nth-child(4) p {
  width: 180px;
}
.text p {
  margin-left: 15px;
}
.verify {
  position: relative;
  left: -94px;
}
</style>
