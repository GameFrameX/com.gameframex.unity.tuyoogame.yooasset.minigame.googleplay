<div align="center">

<img src="https://download.alianblank.com/gameframex/gameframex_logo_320.png" alt="Game Frame X Logo" width="160" />

# GameFrameX YooAsset MiniGame GooglePlay

[![License](https://img.shields.io/github/license/GameFrameX/com.gameframex.unity.tuyoogame.yooasset.minigame.googleplay)](https://github.com/GameFrameX/com.gameframex.unity.tuyoogame.yooasset.minigame.googleplay/blob/main/LICENSE.md)
[![Version](https://img.shields.io/github/v/release/GameFrameX/com.gameframex.unity.tuyoogame.yooasset.minigame.googleplay)](https://github.com/GameFrameX/com.gameframex.unity.tuyoogame.yooasset.minigame.googleplay/releases)
[![Unity Version](https://img.shields.io/badge/Unity-2019.4-black?logo=unity)](https://unity.com/)
[![Documentation](https://img.shields.io/badge/Documentation-docs-blue)](https://gameframex.doc.alianblank.com)

All-in-One Solution for Indie Game Development · Empowering Indie Developers' Dreams

<br />

[Documentation](https://gameframex.doc.alianblank.com) · [Quick Start](#quick-start) · QQ Group: 467608841 / 233840761

<br />

**English** | [简体中文](README.zh-CN.md) | [繁體中文](README.zh-TW.md) | [日本語](README.ja.md) | [한국어](README.ko.md)

</div>

## Project Overview

GameFrameX YooAsset MiniGame GooglePlay runtime component for Unity WebGL platform. Provides adapter implementation for Google Play Mini Game file system and asset bundle loading.

## Features

- Provides Google Play Mini Game specific IFileSystem implementation
- Adapts Google Play Mini Game SDK's AssetBundle download and caching workflow
- Supports package version requests, manifest loading, asset bundle download and loading
- Compatible with remote services and decryption services

## Requirements

- Unity 2019.4
- Platform: UNITY_WEBGL
- Conditional compilation: GOOGLEPLAYMINIGAME
- Dependencies: YooAsset, StarkWebGL, GooglePlayWebGL

## Quick Start

### Installation (choose one)

1. Add the following to the `dependencies` section of your `manifest.json`:
   ```json
   {"com.gameframex.unity.tuyoogame.yooasset.minigame.googleplay": "https://github.com/GameFrameX/com.gameframex.unity.tuyoogame.yooasset.minigame.googleplay.git"}
   ```

2. In Unity's Package Manager, use `Git URL` to add the package: https://github.com/GameFrameX/com.gameframex.unity.tuyoogame.yooasset.minigame.googleplay.git

3. Download the repository and place it in your Unity project's `Packages` directory. It will be loaded automatically.

### Usage

1. Ensure Google Play Mini Game SDK is integrated and `GOOGLEPLAYMINIGAME` macro is enabled
2. Use `GooglePlayFileSystemCreater.CreateFileSystemParameters(...)` to generate file system parameters
3. Pass the parameters to YooAsset's file system creation workflow
4. Follow YooAsset's standard workflow for initialization, version requests, manifest loading, and asset loading

## Documentation & Resources

- [Official Documentation](https://gameframex.doc.alianblank.com)

## Community & Support

- QQ Group: [Join](https://qm.qq.com/q/3dIpogITg)

## Changelog

See [Releases](https://github.com/GameFrameX/com.gameframex.unity.tuyoogame.yooasset.minigame.googleplay/releases) for changelog.

## License

This project is licensed under the MIT License - see the [LICENSE](https://github.com/GameFrameX/com.gameframex.unity.tuyoogame.yooasset.minigame.googleplay/blob/main/LICENSE) file for details.
