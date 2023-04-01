<template>
    <div class="tiktool-body">

        <div class="tiktool-left">
            <div class="tiktool-header">
                <h1>TikTool</h1>
            </div>
            <el-menu class="tiktool-menu" default-active="2" :router="true">
                <div>
                    <el-menu-item index="dasdasd">
                        <i class="el-icon-s-home"></i>
                        <span>首页</span>
                    </el-menu-item>
                </div>
                <div>
                    <el-menu-item index="2">
                        <i class="el-icon-menu"></i>
                        <span>菜单项2</span>
                    </el-menu-item>
                </div>
                <div>
                    <el-menu-item index="3">
                        <i class="el-icon-setting"></i>
                        <span>设置</span>
                    </el-menu-item>
                </div>
            </el-menu>
        </div>
        <el-main class="tiktool-main">
            <!-- 在这里放置你的内容 -->
        </el-main>
    </div>
</template>
  
<style>
body {
    margin: 0;
    padding: 0;
    height: 100%;
    background-color: transparent;
}

.tiktool-body {
    height: 100vh;
    width: 100%;
    display: flex;
    flex-direction: row;
}

.tiktool-left {
    display: flex;
    width: 250px;
    flex-direction: column;
    background-color: rgba(32, 33, 35);
    font-family: 'Roboto Condensed', sans-serif;
    font-size: 16px;
    color: white;
}

.tiktool-left * {
    font-family: 'Roboto Condensed', sans-serif;
    font-size: 16px;
    color: white;
    background-color: rgba(32, 33, 35);
}

.tiktool-header {
    height: 64px;
    display: flex;
    align-items: center;
    justify-content: center;
}

.tiktool-header h1 {
    font-size: 24px;
    font-weight: 700;
    letter-spacing: 2px;
    margin: 0;
}

.tiktool-left .tiktool-menu {
    border: 0px;
}

.tiktool-menu>div {
    padding: 3px 8px;
}

.tiktool-menu .el-menu-item {
    height: 45px;
    border-radius: 10px;
}

.tiktool-menu .el-menu-item * {
    background: transparent;
}

.tiktool-menu .el-menu-item:hover {
    background-color: #2A2B32;
}

.tiktool-menu .el-menu-item.is-active {
    background-color: rgba(52, 53, 65)
}

.tiktool-main {
    flex: 1;
    padding: 20px;
    overflow: auto;
}
</style>
  