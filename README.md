# 城际出行 App 发布仓库

本仓库是「城际出行」App 的发布中枢：
- `config.json` — 远程配置（版本检测 + 下载地址 + 统计上报地址），**改这里 = 改一切**
- Releases — 每个版本的 APK 安装包

## 发新版流程（3步）
1. 打包 APK
2. 上传 GitHub Releases（v1.x 标签）
3. 改 config.json 的 versionCode / versionName / updateNote / apkUrl

用户 app 启动时会自动拉取 config.json 检查更新。
