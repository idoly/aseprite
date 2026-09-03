# Aseprite Windows x64 构建

[![构建 Aseprite](https://github.com/idoly/aseprite/actions/workflows/build.yml/badge.svg)](https://github.com/idoly/aseprite/actions/workflows/build.yml)

这是一个非官方 GitHub Actions 工作流，用于在 Windows x64 环境中验证
[Aseprite](https://github.com/aseprite/aseprite) 的最新稳定版本。

## 功能

- 查询 Aseprite 官方仓库发布的最新稳定版本。
- 使用 GitHub 最新 Windows Runner、MSVC x64、Ninja 和匹配版本的 Skia 进行构建。
- 验证 `aseprite.exe` 的目标架构为 x64。
- 验证程序不依赖 OpenSSL 运行时 DLL。
- 使用 GitHub Actions 缓存记录已成功构建的版本，避免定时任务重复构建。

工作流每天 UTC 03:17 检查一次新版本，并在 `main` 分支发生变更时运行检查。
手动运行工作流时，无论当前版本是否已经构建，都会强制重新构建最新稳定版本。

## 手动运行

1. 打开 [Build Aseprite 工作流](https://github.com/idoly/aseprite/actions/workflows/build.yml)。
2. 点击 **Run workflow**。
3. 等待 `Windows x64` 任务完成。

## 二进制分发

本仓库不会通过 Releases 或 GitHub Actions Artifacts 发布编译后的可执行文件。
Aseprite 允许出于个人用途编译和修改源代码，但其 EULA 限制重新分发编译后的二进制文件。
具体条款请参阅官方 [Aseprite EULA](https://github.com/aseprite/aseprite/blob/main/EULA.txt)。

## 免责声明

本项目与 Igara Studio 或 Aseprite 官方项目没有关联，也未获得其认可。
Aseprite 及其源代码的相关权利归各自权利人所有。
