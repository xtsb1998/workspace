<template>
  <div>
    <div class="container">
      <el-button type="primary" @click="visible = true;">点我弹框</el-button>
    </div>
    <el-dialog v-dialogDrag title="评论" center :visible.sync="visible" width="50%" >
      <el-row :gutter="10" style="height: 30px;margin-bottom: 10px;">
        <el-col :span="11">
          <div class="grid-content bg-purple size" >评论来自：</div>
        </el-col>
        <el-col :span="13">
          <div class="grid-content bg-purple-light size">评论时间：</div>
        </el-col>
      </el-row>
      <el-row :gutter="10">
        <el-col :span="4">
          <div class="grid-content bg-purple size">评论话题：</div>
        </el-col>
        <el-col :span="20">
          <div class="grid-content bg-purple-light text">
            内容内容内容内容内容内容内容内容内容内容
            内容内容内容内容内容内容内容内容内容内容内容内容内容内容内容内容内容内容内容内容
          </div>
        </el-col>
      </el-row>
      <hr>
      <el-row :gutter="10">
        <el-col :span="24">
          <div class="grid-content bg-purple size">政府政策：</div>
        </el-col>
        <el-col :span="24">
          <div class="grid-content bg-purple-light">
            内容内容内容内容内容内容内容内容内容内容
            内容内容内容内容内容内容内容内容内容内容内容内容内容内容内容内容内容内容内容内容
          </div>
        </el-col>
      </el-row>

      <!-- <span slot="footer" class="dialog-footer">
                <el-button @click="visible = false">取 消</el-button>
                <el-button type="primary" @click="visible = false">确 定</el-button>
      </span>-->
    </el-dialog>
  </div>
</template>
<script>
export default {
  data() {
    return {
      visible: false
    };
  }
};
</script>
<style scoped>
/* 弹框一 */
*{
    font-size: 16px
}
.el-dialog__title {
  font-size: 22px;
}
.size {
  font-size: 18px;
  font-weight: 500;
  color: #303133;
  font-family: MicrosoftYaHei-Bold;
}

.el-dialog{
    height: 580px;
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
.el-dialog__body .el-row:last-child>.el-col:nth-child(1){
  margin-bottom: 20px;
}
.el-dialog {
  border-radius: 10px;
}
hr{
    border: 0;
    height: 5px;
    background-color: #EEEEEE;
    margin-bottom: 30px;
}
</style>
