# Aseprite Windows x64 构建

[![构建状态](https://github.com/idoly/aseprite/actions/workflows/build.yml/badge.svg)](https://github.com/idoly/aseprite/actions/workflows/build.yml)

使用 GitHub Actions 编译并验证 [Aseprite](https://github.com/aseprite/aseprite) 最新稳定版。

- 环境：`windows-latest`、MSVC x64、Ninja 和对应版本的 Skia
- 自动：每天检查新版本，已成功构建的版本不会重复构建
- 手动：从 Actions 页面运行时强制重新构建
- 验证：检查 x64 架构，并排除 OpenSSL 运行时 DLL 依赖
- 下载：构建结果在 Actions 运行页面保留 7 天，过期后可手动重新构建

本仓库不创建 Releases。编译产物仅供个人使用，请勿重新分发。具体限制请参阅官方
[Aseprite EULA](https://github.com/aseprite/aseprite/blob/main/EULA.txt)。
