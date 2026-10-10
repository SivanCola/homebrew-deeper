# Deeper Homebrew tap

This repository distributes the CLI cask for
[Deeper](https://github.com/SivanCola/deeper), independently maintained by SivanCola.

本仓库用于发布 Deeper CLI 的 Homebrew cask，由 SivanCola 独立维护。

## Availability / 发布状态

The tap is initialized. `Casks/deeper.rb` will be created by the first stable
Deeper release. Until then, the CLI is not installable from this tap.

tap 已初始化。首次正式稳定发布会自动创建 `Casks/deeper.rb`；在此之前无法通过
这个 tap 安装 CLI。

After the first stable release / 首次稳定发布后：

```sh
brew tap SivanCola/deeper
brew install --cask SivanCola/deeper/deeper
```

## Publishing / 发布维护

Deeper's release workflows update `Casks/deeper.rb` on this repository's `main`
branch. Store the dedicated `HOMEBREW_TAP_TOKEN` secret in `SivanCola/deeper`.
The token needs Contents read/write access to only this tap and the automatically
required Metadata read access. See the
[release setup guide](https://github.com/SivanCola/deeper/blob/main/docs/DEEPER_INDEPENDENCE.md#homebrew-token--homebrew-专用-token).

Deeper 发布工作流更新本仓库的 `main` 分支。专用 Token 只授权本 tap 的 Contents
读写权限，保存在 `SivanCola/deeper` 的 Actions Secret 中；过期前更换。

The tap is MIT licensed. Deeper retains its original license and authorship in
the application repository's LICENSE and NOTICE files.

tap 采用 MIT 许可证；应用本身的原许可证及作者信息保留在主仓库的 LICENSE 和 NOTICE 中。
