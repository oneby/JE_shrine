<template>
  <el-container style="height: 770px;">
  <el-header id="bdHead"> 
      <h1>双谱转换</h1>
        <p>此功能用于简谱和半音阶口琴专用BD谱之间的转换
     PS：请注意BD谱和简谱所放的的位置</p>
    </el-header>
   <el-main>
       <el-row :gutter="20">
  <el-col :span="12">
      <el-input
  type="textarea"
  :rows="23"
  placeholder="请在此处输入"
  v-model="input">
</el-input>
      </el-col>
  <el-col :span="12">
      <el-input
  type="textarea"
  :rows="23"
  placeholder="这里是输出"
  v-model="output">
</el-input>
      </el-col>
</el-row >
  <div id="bdButton">
  <el-button>默认按钮</el-button>
  <el-button type="primary">主要按钮</el-button>
  <el-button type="success">成功按钮</el-button>
  <el-button type="info">信息按钮</el-button>
  <el-button type="warning">警告按钮</el-button>
  <el-button type="danger">危险按钮</el-button>
</div>
    </el-main>
</el-container>
</template>
<script>
  export default {
      data() {
          return {
              output: '',
              input: ''
          }
      }
  }
</script>
<style lang="scss">
#bdHead h1{
    padding-top: 40px;
    font-size: 2em;
}
#bdHead p{
    padding-top: 20px;
    color: #888;
    font-size: 1.3em;
}
#bdHead {
    height: 100px !important;
}
#bdButton{
    padding-top: 50px
}
</style>
