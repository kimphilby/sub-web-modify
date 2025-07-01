<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<style>
/* Global Styles */
body {
  transition: background-color 0.3s, color 0.3s;
}

/* Light Mode */
.light-mode {
  background-image: url('https://tg-image.newsss.workers.dev/file/BQACAgIAAyEGAASKDp_bAANBaDqjsk6x_4iZPvVygAIW5rcS7_gAAu52AAKnntBJtZuXoA3jBYw2BA.jpg');
  background-size: cover;
  background-position: center;
  background-attachment: fixed;
  color: #333;
}

/* Dark Mode */
.dark-mode {
  background-image: url('https://tg-image.newsss.workers.dev/file/BQACAgIAAyEGAASKDp_bAANCaDsNCS7wo13abjf5rf2Tk08cz8cAArlzAAKnnthJrZOBGnSDepw2BA.jpg');
  background-size: cover;
  background-position: center;
  background-attachment: fixed;
  color: #f0f0f0;
}

#app {
  font-family: 'Helvetica Neue', Helvetica, 'PingFang SC', 'Hiragino Sans GB', 'Microsoft YaHei', '微软雅黑', Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  padding: 20px;
}

/* Card Styles */
.el-card {
  border: none !important;
  border-radius: 12px !important;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.05);
  transition: box-shadow 0.3s;
}

.light-mode .el-card {
  background-color: rgba(255, 255, 255, 0.8) !important;
}

.dark-mode .el-card {
  background-color: rgba(38, 38, 38, 0.8) !important;
  color: #f0f0f0 !important;
}

.dark-mode .el-card__header {
    border-bottom: 1px solid #363636;
}


/* Button Styles */
.el-button {
  border-radius: 8px !important;
  transition: all 0.3s;
}

.el-button--primary {
  background-color: #409EFF !important;
  border-color: #409EFF !important;
}
.el-button--primary:hover {
  background-color: #66b1ff !important;
  border-color: #66b1ff !important;
}

.el-button--danger {
    background-color: #F56C6C !important;
    border-color: #F56C6C !important;
}
.el-button--danger:hover {
    background-color: #f78989 !important;
    border-color: #f78989 !important;
}


/* Input Styles */
.el-input__inner, .el-textarea__inner {
  border-radius: 8px !important;
  border: 1px solid;
  transition: border-color 0.3s, box-shadow 0.3s;
}

.light-mode .el-input__inner, .light-mode .el-textarea__inner {
  border-color: #dcdfe6;
}
.light-mode .el-input__inner:focus, .light-mode .el-textarea__inner:focus {
  border-color: #409EFF;
  box-shadow: 0 0 0 2px rgba(64, 158, 255, 0.2);
}

.dark-mode .el-input__inner, .dark-mode .el-textarea__inner {
    background-color: #333;
    border-color: #555;
    color: #f0f0f0;
}
.dark-mode .el-input__inner:focus, .dark-mode .el-textarea__inner:focus {
  border-color: #409EFF;
  box-shadow: 0 0 0 2px rgba(64, 158, 255, 0.2);
}


/* Scrollbar */
::-webkit-scrollbar {
  width: 8px;
  height: 8px;
}
::-webkit-scrollbar-track {
  background: transparent;
}
::-webkit-scrollbar-thumb {
  background: #ccc;
  border-radius: 4px;
}
.dark-mode::-webkit-scrollbar-thumb {
  background: #555;
}
</style>