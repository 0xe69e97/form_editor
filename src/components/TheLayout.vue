<template>
  <div>
    <el-container>
      <el-header>
        表单编辑器
      </el-header>
      <el-main>
        <el-aside>
          左边侧栏
        </el-aside>
          中间内容

        <el-aside>
          右边侧栏
        </el-aside>
      </el-main>
    </el-container>
  </div>
</template>

<script>
export default {
  name: 'TheLayout'
}
</script>

<style lang="scss" scoped>
  .el-container {
    display: flex;
  }
  .el-aside {
    background-color: #999;
    width: 250px;
  }
</style>
