# PCL个人启动器（个人修改版）

本项目是第三方基于 Plain Craft Launcher (PCL) 源码独立修改的个人版本，由 ZexW-wzx 维护，不代表 PCL 官方。

原作者：龙腾猫跃。原项目：https://github.com/Hex-Dragon/PCL2
原作者赞助：https://meloong.com/afd/a/LTCat

## 用途与修改

用于 Windows 上个人学习、构建和运行 Minecraft: Java Edition 启动器。

- 配置本项目自己的 Microsoft OAuth Application (Client) ID，并支持通过 PCL_MS_CLIENT_ID 环境变量覆盖。
- 支持从环境变量或本机独立文件读取 CurseForge API Key；仓库不提供该密钥。
- 调整开源版本的下载地址签名处理。
- 添加适用于 .NET SDK 构建环境的 WPF targets 导入。

## Minecraft Services access request

This is an independently modified personal build of PCL maintained by ZexW-wzx, not an official PCL release.

Application display name: PCL个人启动器
Application (client) ID: 22f84d06-17fc-4a30-bde4-b4774fdcf704

Minecraft Services access is requested to complete Microsoft/Xbox sign-in, obtain a Minecraft access token, verify game ownership, retrieve the Minecraft profile, and launch Minecraft: Java Edition for an authenticated account with a valid entitlement.

The current sign-in flow completes Microsoft OAuth, Xbox Live and XSTS authentication, but Minecraft Services returns HTTP 403 with "Invalid app registration". Application approval has not been verified; this project does not claim to be approved by Microsoft or Mojang.

## 源码与许可

保留上游 LICENCE 和子项目许可证，使用与分发须遵守相应条款。上游介绍见 README.upstream.md。

仓库仅包含项目源码与已有构建资源，不包含本机登录缓存、账号令牌、API 密钥、日志、游戏存档或游戏本体。当前个人构建环境未整理为可复现的构建指南。

