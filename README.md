# Aseprite Windows x64 构建

[![构建状态](https://github.com/idoly/aseprite/actions/workflows/build.yml/badge.svg)](https://github.com/idoly/aseprite/actions/workflows/build.yml)

使用 GitHub Actions 构建 [Aseprite](https://github.com/aseprite/aseprite) 最新稳定版的 Windows x64 程序。

- 每天检查新版本并按需构建，也可手动强制构建
- 每天清理未实际编译的运行记录
- 版本检查使用 Linux runner，实际编译使用 Windows x64 runner
- 构建结果在对应运行页面的 **Artifacts** 中保留 7 天

> [!IMPORTANT]
> 编译产物仅供个人使用，请勿重新分发。详见 [Aseprite EULA](https://github.com/aseprite/aseprite/blob/main/EULA.txt)。
