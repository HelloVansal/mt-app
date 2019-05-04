<template>
  <div class="page-index">
    <el-row>
      <el-col :span="5">
        <emenu/>
      </el-col>
      <el-col :span="19">
        <slider/>
      </el-col>
    </el-row>
    <el-row :span="24">
      3
    </el-row>
  </div>
</template>

<script>
import Emenu from '@/components/index/menu'
import Slider from '@/components/index/slider'
export default {
  components: {
    Emenu,
    Slider
  }
}
</script>

<style lang="scss">
  @import './../assets/css/index/index.scss';
  @import './../assets/css/index/artistic.scss';
  @import './../assets/css/index/life.scss';
</style>
