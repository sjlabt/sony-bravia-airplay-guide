# 索尼电视免费投屏：DLNA + AirPlay 全搞定

一篇实测教程（单页网页，`index.html`）：在一台索尼 Android TV 上，用开源接收器 [MiracastReceiver](https://github.com/weekdayjast/MiracastReceiver) 同时实现——

- **国内 App 投屏（DLNA 推送）**：B 站、优酷、爱奇艺、咪咕等，"投屏"按钮里能找到电视；投上之后手机可以退出，电视自己播
- **AirPlay**：iPhone / iPad / Mac 的屏幕镜像与视频投屏
- （附加）Windows「无线显示器」、安卓系统"投屏"的整屏镜像（视机型支持，索尼自带屏幕镜像的机型无需额外配置）

不用 root、不用 USB 线、没有广告和会员，全程约 15 分钟，装完电脑就可以收起来。

教程：https://sjlabt.github.io/sony-bravia-airplay-guide/

## 这份教程的特点

- **每一步都有验证方法**：写清了"看到什么算成功"，以及出错时怎么一步步排查
- **三个高频坑单独讲**：配对端口 / 连接端口混淆、32 位 64 位选错包、少数机型 AirPlay 列表不显示（含完整修复方案）
- **写给人，也写给 AI**：所有命令、端口、预置参数都明确标注；可以把整页发给 AI，让它带着你一步步操作（教程内附现成的提示词）

## 实测环境

| 项目 | 信息 |
|---|---|
| 设备 | 国行索尼 BRAVIA 4K AE1（系统内设备名 SONY XR-65A95L） |
| 系统 | Android 14（SDK 34），CPU 为 32 位（armeabi-v7a） |
| 软件 | MiracastReceiver v1.2.5 |
| 日期 | 2026-10-12 |

> 其他机型请以你自己电视上读到的信息为准（教程内有读取命令），方法通用。

## 安全提醒

- APK 只从官方 Release 下载（教程内有链接和 SHA-256 校验方法），不要用来路不明的安装包
- 不要在任何路由器上把 ADB 端口映射到公网

## 致谢

- [weekdayjast/MiracastReceiver](https://github.com/weekdayjast/MiracastReceiver)（MIT 协议）——教程使用的开源接收器，好用的话去项目点个 Star
- [索尼 BRAVIA 5 免费 AirPlay 实战](https://shuimu2000.github.io/sony-bravia-free-airplay-guide.html)——本教程的起点；那篇用的是另一款只做 AirPlay 的开源方案，只想投 iPhone 的也可以直接看它

## 免责

本仓库为个人经验分享，步骤按上述实测环境整理。按教程操作属于自主行为，请只调试自己拥有或有权管理的设备。
