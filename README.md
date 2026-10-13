CroHAC 网站源码，通过 GitHub Pages 发布，网站为 [crohac.github.io](https://crohac.github.io/)。

这是一个无需构建步骤的静态网站，入口为 `index.html`。`.nojekyll` 让 GitHub Pages 直接发布静态文件。

发布源使用 `main` 分支的根目录。初始化后，修改网页并推送到 `main`，GitHub Pages 会自动更新网站。

本地预览可在仓库目录运行：

```sh
python3 -m http.server 8000 --bind 127.0.0.1
```

然后访问 [本地预览](http://127.0.0.1:8000/)。

本机提交身份仅配置在本仓库的 `.git/config`，使用 `CroHAC` 和对应的 GitHub 隐私邮箱。推送认证使用仅授权此仓库的独立 SSH Deploy key，私钥保存在本机 `.git` 目录中，不会提交或发布。

本项目不修改全局 Git 配置、默认 GitHub CLI 账号或 `~/.ssh/config`。其他设备克隆后需要自行配置提交身份与认证。

本仓库仅存放网站文件，工作目录中的论文、草稿和组织材料不属于发布内容。
