# ACT哮喘控制测试 - GitHub Pages 部署指南

## 📦 文件说明

| 文件 | 说明 |
|------|------|
| `index.html` | ACT哮喘控制测试页面（主文件）|

## 🚀 部署步骤（3分钟完成）

### 第一步：创建 GitHub 仓库

1. 登录 [GitHub](https://github.com)
2. 点击右上角 **+** → **New repository**
3. 填写仓库名称，例如：`act-asthma-test`
4. 选择 **Public**（公开）
5. 点击 **Create repository**

### 第二步：上传文件

**方式A：网页上传（推荐新手）**

1. 在新创建的仓库页面，点击 **uploading an existing file**
2. 将 `index.html` 文件拖拽到上传区域
3. 点击 **Commit changes**

**方式B：命令行上传**

```bash
# 克隆仓库（替换为你的用户名和仓库名）
git clone https://github.com/你的用户名/act-asthma-test.git
cd act-asthma-test

# 复制文件
cp /path/to/index.html .

# 提交
 git add .
git commit -m "Add ACT asthma test"
git push origin main
```

### 第三步：开启 GitHub Pages

1. 在仓库页面，点击 **Settings**
2. 左侧菜单选择 **Pages**
3. **Source** 选择 **Deploy from a branch**
4. **Branch** 选择 **main**，文件夹选 **/(root)**
5. 点击 **Save**
6. 等待 1-2 分钟，页面会显示访问链接：
   ```
   https://你的用户名.github.io/act-asthma-test/
   ```

## 📱 生成二维码

得到链接后，用任意二维码生成工具生成二维码：

- 在线工具：[草料二维码](https://cli.im)、[QR Code Generator](https://www.qr-code-generator.com)
- 微信扫一扫：把链接发给自己，用微信内置二维码生成

## ✅ 完成！

用户扫码即可使用，无需审核，完全免费！

## 🔗 访问地址示例

```
https://zhangsan.github.io/act-asthma-test/
```

## 📝 自定义域名（可选）

如果想用自己的域名（如 `act.yourdomain.com`）：

1. 在仓库根目录创建 `CNAME` 文件，内容写你的域名
2. 在域名DNS设置中添加 CNAME 记录指向 `你的用户名.github.io`
3. 在 GitHub Pages 设置中填入自定义域名

## 🆘 常见问题

**Q: 页面打开是404？**  
A: 等待 2-3 分钟让 GitHub Pages 部署完成，或检查文件名是否为 `index.html`

**Q: 可以用私有仓库吗？**  
A: 可以，但 GitHub Pages 只有 Pro 用户才能用于私有仓库

**Q: 如何更新内容？**  
A: 直接修改 `index.html` 并重新上传提交，自动更新