<template>
  <div class="slider">
    <el-row :gutter="10" class="up">
      <el-col :span="15">
        <div class="big"></div>
      </el-col>
      <el-col :span="3">
        <div class="life"></div>
      </el-col>
      <el-col :span="6">
        <div class="login"></div>
      </el-col>
    </el-row>
  </div>
</template>

<script>
export default {
  name: 'slider'
}
</script>

<style lang="scss" scoped>
  .slider {
    .up {
      padding: 10px 0 10px 10px;
      .big {
        height: 240px;
        background-image: url('http://p0.meituan.net/codeman/e473bb428f070321269b23370ff02ba956209.jpg');
        background-size: 100% 100%;
      }
      .life {
        height: 240px;
        background-image: url('http://p0.meituan.net/codeman/e473bb428f070321269b23370ff02ba956209.jpg');
        background-size: 100% 100%;
      }
      .login {
        height: 240px;
        background-image: url('http://p0.meituan.net/codeman/e473bb428f070321269b23370ff02ba956209.jpg');
        background-size: 100% 100%;
      }
    }
  }
</style>
