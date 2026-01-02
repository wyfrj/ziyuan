# GitHub 部署指南

按照以下步骤将个人资源小站部署到GitHub Pages：

## 1. 创建GitHub仓库

1. 登录您的GitHub账号
2. 点击右上角"+" → "New repository"
3. 输入仓库名称（如"personal-resource-site"）
4. 选择"Public"（公开）
5. 勾选"Add a README file"
6. 点击"Create repository"

## 2. 上传文件

### 方法一：网页上传（推荐）

1. 在仓库页面点击"Add file" → "Upload files"
2. 将本文件夹中的所有内容拖到上传区域
3. 点击"Commit changes"提交更改

### 方法二：使用Git命令行

1. 确保已安装Git
2. 打开终端/命令行，导航到本文件夹
3. 执行以下命令：

```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/[您的用户名]/[仓库名].git
git push -u origin main
```

## 3. 启用GitHub Pages

1. 进入仓库的"Settings"
2. 左侧选择"Pages"
3. 在"Source"下选择：
   - Branch: main
   - Folder: / (root)
4. 点击"Save"
5. 等待几分钟让GitHub部署

## 4. 访问您的网站

部署完成后，您的网站将可以通过以下URL访问：
```
https://[您的用户名].github.io/[仓库名]/
```

## 5. 更新网站

如需更新网站内容：

1. 修改文件后，重新上传/提交更改
2. GitHub会自动重新部署（可能需要几分钟）

## 注意事项

- 确保所有文件路径正确
- 首次部署可能需要10-15分钟
- 如果遇到问题，检查浏览器控制台是否有错误
