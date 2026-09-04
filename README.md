# Aria Magic Voice 全平台安装包分发仓库

本仓库为 **Aria Magic Voice** 官方内测与体验包专用分发归档库。

> **核心原则**：
> 1. 本仓库 Git 分支仅存放各平台说明、最新版本元数据指针（Manifest）与 SHA256 校验指纹，**不把大型安装包（DMG/APK/IPA）提交入 Git 分支**。
> 2. 所有正式与内测安装包均挂载在对应的 **GitHub Releases** 附件中分发。
> 3. 各平台保持独立生命周期与 Tag 体系，互不干扰。

---

## 平台索引导航

| 平台目录 | 支持系统 | 产品形态 | 当前推荐分发通道 | Release 命名规范 |
|---|---|---|---|---|
| [**`macos/`**](./macos/README.md) | macOS 14.0+ (Apple Silicon) | 原生输入法 (IME) / DMG | 官网 Developer ID 公证直发 / GitHub Releases | `AriaInputMethod-macOS-v<version>.dmg` |
| [**`android/`**](./android/README.md) | Android 10.0+ (ARM64) | 原生输入法服务 (IME) / APK | GitHub Releases / 百度网盘 / 谷歌Drive | `AriaInputMethod-Android-v<version>.apk` |
| [**`ios/`**](./ios/README.md) | iOS 17.0+ | 输入法扩展 / TestFlight | Apple TestFlight / App Store 官方渠道 | 官方 TestFlight 指针 |

---

## 验证与安全性

为保障用户设备绝对安全，所有安装包发布前均完成以下校验：
- **SHA256 校验**：每个发布的附件均在对应平台目录下提供实时哈希指纹，防止任何网络劫持或下载损坏。
- **隐私保护原则**：所有语音识别与文本处理 100% 本地离线完成，绝不上传私密内容。
