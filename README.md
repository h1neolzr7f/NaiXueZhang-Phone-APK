# Nai 学长工作室 Android APK

这个仓库只维护安装包的分发说明和校验信息。公开源码在 [NaiXueZhang-Phone](https://github.com/h1neolzr7f/NaiXueZhang-Phone)，Windows 版在 [NaiXueZhang-Studio-Upgrade](https://github.com/h1neolzr7f/NaiXueZhang-Studio-Upgrade)。

## 当前安装包

| 项目 | 值 |
|---|---|
| 版本 | `1.5.2-phone.23` |
| versionCode | `174` |
| 包名 | `com.naixuezhang.studio.mobile` |
| ABI | `arm64-v8a`（仅 64 位 Android） |
| 文件大小 | `52,819,220` bytes |
| SHA-256 | `213ddd93005a70284c05d3e978734d13cd086d492d6f3fa6ae9ed2f5b19e9095` |
| 签名 | debug |

[临时下载镜像](https://litter.catbox.moe/mukoxq.apk)可能在约 72 小时后失效。下载后务必核对 SHA-256；无法核对或校验不一致时不要安装。

PowerShell：

```powershell
Get-FileHash .\NaiXueZhang-Phone-1.5.2.apk -Algorithm SHA256
```

由于当前包使用 debug 签名，从不同签名的旧版升级通常会失败，需要先导出自己的数据并卸载旧版。安装未知来源 APK 会扩大设备风险面，只应在理解来源和权限的设备上操作。

## 源码与二进制关系

公开源码默认分支目前是 phone.16，分发 APK 是 phone.23，因此还不是可复现的一一对应关系。不要把“源码可见”写成“当前 APK 已由该提交可复现构建”。后续发布应改用 GitHub Release 固定资产，并在 Release 说明中同时记录源码 commit、签名和 SHA-256。

应用需要使用者自行提供第三方服务凭据。Token 和 API Key 只应在应用设置里填写，不要发到 Issue、日志或截图中。

这是非官方项目，与 pixiv Inc.、NovelAI/Anlatan、AITag、DeepSeek 或其他第三方服务没有隶属、授权或合作关系。
