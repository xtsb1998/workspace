<template>
  <div class="container">
    <el-row>
      <el-col :span="2">网站名称：</el-col>
      <el-col :span="6">智慧社区管理后台</el-col>
    </el-row>

    <el-row>
      <el-col :span="2">电话：</el-col>
      <el-col :span="6">027-88888888</el-col>
    </el-row>

    <el-row>
      <el-col :span="2">地址:</el-col>
      <el-col :span="6">
        <el-input placeholder="请输入地址" v-model="input0"></el-input>
      </el-col>
    </el-row>
    <el-row>
      <el-col :span="2">邮编:</el-col>
      <el-col :span="6">
        <el-input placeholder="请输入邮编" v-model="input1"></el-input>
      </el-col>
    </el-row>
    <el-row>
      <el-col :span="2">信息归属:</el-col>
      <el-col :span="6">
        <el-input placeholder="请输入信息归属" v-model="input2"></el-input>
      </el-col>
    </el-row>
    <el-row>
      <el-col :span="2">技术支持:</el-col>
      <el-col :span="6">
        <el-input placeholder="请输入技术支持" v-model="input3"></el-input>
      </el-col>
    </el-row>
    <el-row>
      <el-col :span="2">客服:</el-col>
      <el-col :span="6">
        <el-input placeholder="请输入客服" v-model="input4"></el-input>
      </el-col>
    </el-row>
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
.el-row{
    line-height: 92px;
    font-size: 18px;
}
</style>