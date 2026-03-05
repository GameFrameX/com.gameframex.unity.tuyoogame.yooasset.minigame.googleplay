## 概述

GameFrameX 的 YooAsset Google Play 小游戏运行时组件，面向 Unity WebGL 平台，提供与 Google Play 小游戏文件系统、资源包加载流程的适配实现。

## 功能特性

- 提供 Google Play 小游戏专用的 IFileSystem 实现
- 适配 Google Play 小游戏 SDK 的 AssetBundle 下载与缓存流程
- 支持包版本请求、清单加载、资源包下载与加载
- 可对接远程服务与解密服务

## 运行环境

- Unity 2019.4
- 平台：UNITY_WEBGL
- 条件编译：GOOGLEPLAYMINIGAME
- 依赖：YooAsset、StarkWebGL、GooglePlayWebGL

## 安装方式（任选其一）

1. 在 `manifest.json` 的 `dependencies` 中添加
   ```json
   {
     "com.gameframex.unity.tuyoogame.yooasset.minigame.googleplay": "https://github.com/gameframex/com.gameframex.unity.tuyoogame.yooasset.minigame.googleplay.git"
   }
   ```
2. 在 Unity 的 Package Manager 使用 Git URL 添加  
   https://github.com/gameframex/com.gameframex.unity.tuyoogame.yooasset.minigame.googleplay.git
3. 直接下载仓库放到 Unity 项目的 `Packages` 目录

## 使用说明

1. 确保已接入 Google Play 小游戏 SDK，并启用 `GOOGLEPLAYMINIGAME` 宏
2. 通过 `GooglePlayFileSystemCreater.CreateFileSystemParameters(...)` 生成文件系统参数
3. 将参数传入 YooAsset 的文件系统创建流程
4. 按照 YooAsset 的常规流程进行初始化、版本请求、清单加载与资源加载

## 主要类型

- `GooglePlayFileSystem`：Google Play 小游戏文件系统实现
- `GooglePlayFileSystemCreater`：文件系统参数构建入口
- `LoadGooglePlayAssetBundleOperation`：资源包下载与加载操作
- `UnityGooglePlayAssetBundleRequestOperation`：基于 Google Play 小游戏 SDK 的下载请求封装

## 注意事项

- 需要设置 Google Play 小游戏的缓存根目录，否则会抛出异常
- 未配置远程服务时会回退到 Web 服务器路径
