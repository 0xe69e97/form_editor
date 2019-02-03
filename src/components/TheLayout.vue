<template>
  <div class="main-page">
    <el-container>
      <el-header>
        表单编辑器
      </el-header>
      <el-main>
        <el-aside>
          <the-left />
        </el-aside>
          <the-main />
        <el-aside>
          <the-right />
        </el-aside>
      </el-main>
      <el-footer>
        Smalin @ 2019
      </el-footer>
    </el-container>
  </div>
</template>

<script>
import TheLeft from '@/components/TheLeft.vue'
import TheRight from '@/components/TheRight.vue'
import TheMain from '@/components/TheMain.vue'
export default {
  name: 'TheLayout',
  components: {
    TheLeft,
    TheRight,
    TheMain
  }
}
</script>

<style lang="scss" scoped>
  .main-page {
    width: 100vw;
    height: 100vh;
  }
  .el-header {
    height: 60px;
    line-height: 60px;
    width: 100vw;
    background-color: rgba(255, 255, 255, 0.8);
    box-sizing: border-box;
    border-bottom: 1px solid #eaecef;
  }
  .el-main {
    width: 100vw;
    height: 100%;
    display: flex;
  }
  .el-aside {
    background-color: #999;
    width: 250px;
  }
  .el-footer {
    height: 30px!important;
    line-height: 30px;
    text-align: center;
    color: white;
    background-color: rgba(0, 0, 0, 0.5)
  }
</style>
