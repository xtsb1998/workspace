<template>
  <div>
    <div class="container">
      <el-button type="primary" @click="visible = true;">点我弹框</el-button>
    </div>
    <el-dialog v-dialogDrag title="新闻详情" center :visible.sync="visible" width="50%">
      <el-row :gutter="10">
        <el-col>
          <div class="grid-content bg-purple size">活动标题</div>
        </el-col>
        <el-col>
          <div class="grid-content bg-purple-light">
            <img src="./zhunze.png" alt="活动图片" width="100%" height="150px" />
          </div>
        </el-col>
        <el-col>
          <div
            class="grid-content bg-purple-light"
            style="color:#A1A1A1;padding:5px;line-height:26px"
          >
            详情详情详情详情详情详情详情详情详情详情详情详情详情详情详情详情详情详情详情
            详情详情详情详情详情详情详情详情详情详情详情详情详情详情详情详情详情详情详情
            详情详情详情详情详情详情详情详情详情详情详情详情详情详情详情详情
          </div>
        </el-col>
      </el-row>
      <el-row :gutter="10" style="margin-bottom:10px">
        <el-col :span="3">
          <div class="grid-content bg-purple-light text" style="line-height: 35px">已报名</div>
        </el-col>
        <el-col :span="14">
          <div class="grid-content bg-purple size">
            <el-progress
              :text-inside="true"
              :stroke-width="35"
              :percentage="70"
              style="color:#FA7224"
            ></el-progress>
          </div>
        </el-col>
        <el-col :span="4">
          <div class="grid-content bg-purple-light text" style="line-height: 35px">总人数</div>
        </el-col>
        <el-col :span="3">
          <div class="grid-content bg-purple-light text" style="line-height: 35px;">
            <i class="el-icon-lx-favor" style="font-size:30px"></i><span>1566</span>
          </div>
        </el-col>
        <el-col :span="8" :offset="8">
          <el-button
            type="danger"
            style="width:100%;height:30px;margin-top:30px;margin-bottom:10px"
          >立即参加</el-button>
        </el-col>
      </el-row>
      <hr style="height: 10px;margin-bottom: 18px;" />
      <el-row :gutter="10" style="height:170px">
        <el-col>
          <div class="grid-content bg-purple title">评论</div>
        </el-col>
        <el-col :span="2">
          <div style="width:56px;height:56px;border-radius:28px;background-color:#333"></div>
        </el-col>
        <el-col :span="22">
          <el-col :span="4"><div class="title">苏大强弟弟</div></el-col>
          <el-col :span="3"><div style="color:#A1A1A1;font-size:12px">今天15：03{{time}}</div></el-col>
          <el-col :span="3" :offset="13"><i class="el-icon-lx-favor" style="font-size:30px"></i><span>1566</span></el-col>
          <el-col :span="22">
            <div
              class="grid-content bg-purple-light"
              style="color:#A1A1A1;line-height:20px;font-size:14px"
            >
              内容内容内容内容内容内容内容内容内容内容
              内容内容内容内容内容内容内容内容内容内容内容内容内容内容内容内容内容内容内容内容
              内容内容内容内容内容内容内容内容内容内容
              内容内容内容内容内容内容内容内容内容内容内容内容内容内容内容内容内容内容内容内容
              内容内容内容内容内容内容内容内容内容内容
            </div>
            <hr style="height:1px">
          </el-col>
          
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
<style >
/* 弹框一 */
* {
  font-size: 16px;
}
.el-dialog__title {
  font-size: 22px;
}
.size {
  font-size: 14px;
  font-weight: 500;
  color: #303133;
  font-family: MicrosoftYaHei-Bold;
  margin-bottom: 10px;
}
.title {
  font-size: 18px;
  color: #303133;
  
}
.el-dialog {
  height: 700px;
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
  height: 600px;
  overflow: hidden;
}
.el-dialog__body .el-row {
  height: 105px;
}
.el-dialog__body .el-row:nth-child(1) {
  height: 290px;
  margin-bottom: 0px;
}
.el-dialog__body .el-row:last-child > .el-col:nth-child(1) {
  margin-bottom: 20px;
}
.el-dialog {
  border-radius: 10px;
}
hr {
  border: 0;
  background-color: #eeeeee;
}

</style>
