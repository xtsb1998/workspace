<template>
  <section class="main">
    <div class="crumbs">
      <el-breadcrumb separator="/">
        <el-breadcrumb-item>
          <i class="el-icon-rank"></i> 拖拽组件
        </el-breadcrumb-item>
        <el-breadcrumb-item>拖拽弹框</el-breadcrumb-item>
      </el-breadcrumb>
    </div>
    <div class="container">
      <p>通过指令 v-dialogDrag 使 Dialog 对话框具有可拖拽的功能。</p>
      <br />
      <el-button type="primary" @click="visible = true;">点我弹框</el-button>
    </div>
    <el-dialog v-dialogDrag title="政务服务" center :visible.sync="visible" width="50%">
      <el-row :gutter="10">
        <el-col :span="22">
          <div class="grid-content bg-purple size">职业介绍和就业政策质询</div>
        </el-col>
        <el-col :span="2">
          <div class="grid-content bg-purple-light">06/23</div>
        </el-col>
      </el-row>
      <el-row :gutter="10">
        <el-col :span="24">
          <div class="grid-content bg-purple title">政府政策</div>
        </el-col>
        <el-col :span="24">
          <div class="grid-content bg-purple-light">
            内容内容内容内容内容内容内容内容内容内容
            内容内容内容内容内容内容内容内容内容内容内容内容内容内容内容内容内容内容内容内容
          </div>
        </el-col>
      </el-row>
      <el-row :gutter="10">
        <el-col :span="24">
          <div class="grid-content bg-purple title">办理流程</div>
        </el-col>
        <el-col :span="24">
          <div class="grid-content bg-purple-light">
            内容内容内容内容内容内容内容内容内容内容
            内容内容内容内容内容内容内容内容内容内容内容内容内容内容内容内容内容内容内容内容
          </div>
        </el-col>
      </el-row>
      <el-row :gutter="10">
        <el-col :span="24">
          <div class="grid-content bg-purple title">电话咨询</div>
        </el-col>
        <el-col :span="24">
          <div class="grid-content bg-purple-light">027-88888888</div>
        </el-col>
      </el-row>

      <!-- <span slot="footer" class="dialog-footer">
                <el-button @click="visible = false">取 消</el-button>
                <el-button type="primary" @click="visible = false">确 定</el-button>
      </span>-->
    </el-dialog>
  </section>
</template>

<script>
export default {
  data() {
    return {
      visible: false
    };
  },
  
};
</script>

<style scoped>
*{
    font-size: 16px
}
/* 弹框一 */
.el-dialog__title {
  font-size: 22px;
}
.size {
  font-size: 22px;
  font-weight: 500;
  color: #303133;
  font-family: MicrosoftYaHei-Bold;
}
.title {
  margin-bottom: 10px;
  border-left: solid 6px #4c85d2;
}

.el-row {
  margin-bottom: 20px;
  line-height: 20px;
}
.el-row:last-child {
  margin-bottom: 0;
}
.el-header,
.el-footer {
  color: #333;
  line-height: 10px;
  height: 20px !important;
}
.el-main {
  color: #333;
  line-height: 10px;
  /* padding: 0 10px; */
}
.el-dialog__body {
  font-size: 16px;
}
.el-dialog__body .el-row {
  height: 100px;
}
.el-dialog__body .el-row:nth-child(1) {
  height: 40px;
}
.el-dialog__body .el-row .el-col:nth-child(2) {
  padding-left: 14px !important;
}
.el-dialog {
  border-radius: 10px;
}
</style>
