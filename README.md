# QQMusic Android
独立的 Android 音乐播放器实验项目，参考 Spotify 风格交互及开源项目 Melodia、Melodist 和 QQMusicApi，**非腾讯 QQ 音乐官方产品**。

## 项目状态（2026-11-19）
已创建私有仓库并准备 GitHub Actions 构建工作流。目前仓库中的完整 Android 源码**尚未上传**，因此不能声称 APK 已完成。
之前生成的 QQMusic v0.3.1 源码压缩包仍可在原 ChatGPT 对话中下载。

## 下一步
把 QQMusic-v0.3.1-GitHub-ready-source.zip **解压后的文件**上传至仓库根目录（不是直接上传 ZIP）。确认有 `app/`、`build.gradle.kts`、`settings.gradle.kts`。
提交后 Actions 会自动构建；成功后可以在 `Android APK` 运行的 Artifacts 中下载 APK。

## 功能及限制
当前实验版重点为本地播放、歌曲收藏、歌单、歌词以及公开 QQ 音乐曲目查询。
QQ 音乐正式账户、VIP 流媒体和同步等服务尚未实现，不提供破解 DRM 或绕过授权的实现。

第三方仓库许可证：Melodia (MIT)、Melodist (MIT)、QQMusicApi (GPL-3.0-or-later)。请遵守第三方版权、商标和许可证。
