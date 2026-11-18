# Amazon Ads 原型中心

仅存放可公开的 HTML 原型与静态依赖，不同步业务数据、知识库或账号信息。

## 首次发布

1. 在个人 GitHub 账号下创建公开仓库 `amazon-ads-prototypes`。
2. 将本目录中的文件上传到仓库根目录，包括 `.nojekyll`。
3. 在仓库 Settings → Pages 中，选择 Deploy from a branch，分支 `main`，目录 `/ (root)`，保存。
4. 以 Pages 页面显示的实际链接为准，等待发布成功后打开验证。

## 添加和更新原型

将可公开的原型及其依赖放进 `pages/`，保留文件之间的相对路径。运行：

```powershell
powershell -NoProfile -ExecutionPolicy Bypass -File .\Update-Index.ps1
```

脚本根据 `pages/` 内的 HTML 生成首页目录。将更新后的目录上传到同一仓库，Pages 会在提交后更新。相同路径的原型链接保持不变。脚本不会自动上传或连接账户。

外部链接、API、iframe 和资源路径需要在公开环境中另行验证。不要上传真实账号数据、密钥或含业务信息的浏览器缓存。
