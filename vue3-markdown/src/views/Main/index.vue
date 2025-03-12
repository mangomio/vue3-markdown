<template>
  <h1 class="title">基于vue3的markdown文本编辑器</h1>
  <div class="markdown-body">
    <div class="header">头部</div>
    <div class="edit-container">
      <el-scrollbar height="400px">
        <textarea class="edit"></textarea>
      </el-scrollbar>
      <el-scrollbar height="400px">
        <div class="show"></div>
      </el-scrollbar>
    </div>
  </div>
</template>

<script setup></script>

<style scoped lang="scss">
.title {
  text-align: center;
  margin: 20px 0;
}
.markdown-body {
  display: flex;
  flex-direction: column;
  align-items: center;
  width: 100%;
  max-width: 1200px;
  margin: 0 auto;
}

.header {
  width: 100%;
  text-align: center;
  margin-bottom: 20px;
}
.edit-container {
  display: flex;
  width: 100%;
  gap: 20px;
  .edit {
    width: 600px;
    height: 700px;
    resize: none;
    outline: none;
    border: 1px solid #ddd;
    border-radius: 6px;
    padding: 30px;
  }
  .show {
    width: 600px;
    height: 700px;
    border: 1px solid #ddd;
    border-radius: 6px;
    background-color: #fff;
  }
}
</style>
