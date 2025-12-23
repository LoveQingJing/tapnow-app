# TapNow 矩阵控制台 - 打包指南

## 方法一：使用 GitHub 自动打包（推荐，无需安装任何软件）

### 第1步：注册GitHub账号
1. 打开 https://github.com
2. 点击右上角 "Sign up" 注册账号（如已有账号跳过此步）

### 第2步：创建新仓库
1. 登录GitHub后，点击右上角 "+" → "New repository"
2. Repository name 填写：`tapnow-app`
3. 选择 "Public"
4. 点击 "Create repository"

### 第3步：上传文件
1. 在新建的仓库页面，点击 "uploading an existing file"
2. 把本压缩包解压后的所有文件拖进去（包括 .github 文件夹）
   - main.js
   - index.html
   - package.json
   - .github/workflows/build.yml
3. 点击 "Commit changes"

### 第4步：等待自动打包
1. 点击仓库顶部的 "Actions" 标签
2. 你会看到 "Build Windows EXE" 正在运行（黄色圆圈）
3. 等待变成绿色勾（约3-5分钟）

### 第5步：下载EXE
1. 点击绿色勾的那条记录
2. 页面底部找到 "Artifacts"
3. 点击 "TapNow-Windows-EXE" 下载
4. 解压后即可运行！

---

## 方法二：本地打包（需要安装Node.js）

### 前提条件
- 安装 Node.js：https://nodejs.org （下载LTS版本，一路下一步安装）

### 打包步骤
1. 解压本压缩包
2. 在文件夹内空白处，按住Shift + 右键 → "在此处打开PowerShell"
3. 依次执行：
```
npm install
npm run build
```
4. 打包完成后，EXE在 `dist` 文件夹中
