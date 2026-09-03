# Aseprite Windows x64 Build

[![Build Aseprite](https://github.com/idoly/aseprite/actions/workflows/build.yml/badge.svg)](https://github.com/idoly/aseprite/actions/workflows/build.yml)

Unofficial GitHub Actions workflow that verifies the latest stable
[Aseprite](https://github.com/aseprite/aseprite) release on Windows x64.

## What It Does

- Checks the latest stable release published by the official Aseprite repository.
- Builds with the latest GitHub-hosted Windows runner, MSVC x64, Ninja, and the matching Skia package.
- Verifies that `aseprite.exe` targets x64.
- Verifies that the executable does not depend on OpenSSL runtime DLLs.
- Records successful versions in the GitHub Actions cache to avoid duplicate scheduled builds.

The workflow checks for a new stable version every day at 03:17 UTC. It also
runs after changes to `main`. A manual run always rebuilds the latest stable
version.

## Run Manually

1. Open the [Build Aseprite workflow](https://github.com/idoly/aseprite/actions/workflows/build.yml).
2. Select **Run workflow**.
3. Wait for the `Windows x64` job to finish.

## Binary Distribution

This repository does not publish compiled executables through Releases or
GitHub Actions artifacts. Aseprite permits compiling and modifying its source
for personal use, but its EULA restricts redistribution of compiled binaries.
See the official [Aseprite EULA](https://github.com/aseprite/aseprite/blob/main/EULA.txt)
for the applicable terms.

## Disclaimer

This project is not affiliated with or endorsed by Igara Studio or the
Aseprite project. Aseprite and its source code belong to their respective
copyright holders.
