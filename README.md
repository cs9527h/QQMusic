# QQMusic 安卓客户端

此仓库是第三方 Android 原生音乐客户端实验项目，与腾讯 QQ 音乐及 Spotify 无官方关联。

## 一次上传，自动构建 APK

当前 GitHub 工具只能提交文本文件，尚未将上一版源码 ZIP 上传本仓库。为了简化手机操作，已准备好 **自动解压源码 ZIP、编译并上传 APK** 的 GitHub Actions 工作流。

1. 从原 ChatGPT 对话下载 `QQMusic-v0.3.1-GitHub-ready-source.zip`。
2. 在 GitHub 仓库根目录点击 **Add file → Upload files**，直接上传 ZIP，**不要解压**，保持文件名不变，然后 Commit。
3. 自动触发 [Android APK](../../actions/workflows/android.yml)；成功后进入对应运行，在 Artifacts 中下载 `QQMusic-v0.3.1-debug-APK`。

构建时会校验 `app/` 与 Gradle 文件齐全，并运行单元测试与 APK 编译。失败时需根据 Actions 日志修复，当前尚未声称 APK 编译成功。

## 当前功能边界

此版本实现的是本地音乐播放、歌单收藏、歌词解析及公开 QQ 音乐搜索等实验功能。QQ 音乐正式账号、VIP 在线音频、云歌单同步尚未验证或实现。未经授权不会破解 DRM 或绕过会员限制。

参考项目：Melodia（MIT）、Melodist（MIT）、QQMusicApi（GPL-3.0-or-later）。尊重第三方代码许可与品牌标识权利。
