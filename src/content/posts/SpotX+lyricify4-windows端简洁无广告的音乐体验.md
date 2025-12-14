---
title: SpotX+lyricify4-windows端简洁无广告的音乐体验
published: 2025-12-14
description: 'SpotX+lyricify4-windows端简洁无广告的音乐体验'
image: '/src/assets/images/spotify.png'
tags: [Spotify, lyricify4]
category: '软件'
draft: false 
lang: 'zh_CN'
---

## 前言
作为一名音乐爱好者，我一直在寻找一款简洁无广告的在线流媒体服务。之前使用过网易云音乐、QQ音乐等，但是软件过于臃肿，广告太多，体验不佳，甚至开会员都无法关闭广告。手机和MAC上使用apple music,但是windows上apple music体验不佳。所以重新安装Spotify,众所周知国内用户为Spotify付费极为不便,破解去广告也是不得已而为之。

## 什么是SpotX？
[SpotX](https://github.com/SpotX-Official/SpotX)是一款基于Spotify的第三方客户端，windows上一键安装并解锁播放限制，移除广告。

## 什么是lyricify4？
[lyricify4](https://lyricify.app/)是一款歌词显示插件，它可以让用户在Spotify中显示歌词，并且支持多种歌词格式。

## 安装SpotX
推荐安装新主题，旧主题已经不再维护。
终端输入以下命令安装：输入后回车即可，播客和阻止更新看个人需求。
```powershell
iex "& { $(iwr -useb 'https://raw.githubusercontent.com/SpotX-Official/SpotX/refs/heads/main/run.ps1') } -new_theme"
```
![spotX](/src/assets/images/spotX.png)

## 安装lyricify4

如果不知道该在 GitHub releases 里下载哪个版本，建议直接通过微软应用商店一键安装 lyricify4，选择免费试用即可。

如果需要通过 GitHub releases 下载 [lyricify4](https://github.com/WXRIW/Lyricify-App/releases)，推荐所有用户下载 Lyricify Setup (.exe)，而不是 Lyricify (.7z)（如果安装遇到问题，可以尝试下载 Lyricify (.7z) 绿色版）。注意不要下载 pack-update 或 pack-full，这些是自动更新用的，并非完整安装包。

关于文件名选择：
- “x86”, “x64”, “arm64”对应不同设备架构，目前绝大多数设备选“x64”。
- .exe 为安装包；.7z 为绿色免安装版（带 self-contained 的版本自带 .NET 6.0 Desktop Runtime，详情可查阅）；.Portable.7z 为便携版。

如有疑惑，优先选择“Lyricify Setup x64.exe”安装即可。

我安装的是便携版本的，需要下载后解压到文件夹中，然后运行Lyricify.exe即可。
第一次运行可能需要下载.net 6.0 Desktop Runtime，下载后运行即可。

![lyricify](/src/assets/images/lyricify.png)
选择好配置后点击继续会跳转网页授权，看到授权成功页面就大功告成了。
![lyricify授权](/src/assets/images/lyricify授权.png)

## 愉快地使用Spotify吧
现在你的spotify已经可以正常使用了，无广告随意切歌。
![spotify](/src/assets/images/spotify.png)
当然还有lyricify4的歌词显示，支持多种歌词格式。
![lyricify歌词](/src/assets/images/lyricify歌词.png)