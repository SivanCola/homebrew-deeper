# Deepzora Homebrew tap

This repository distributes the CLI cask for
[Deepzora](https://github.com/SivanCola/deepzora), independently maintained by SivanCola.

本仓库用于发布 Deepzora CLI 的 Homebrew cask，由 SivanCola 独立维护。

## Availability / 发布状态

The tap is initialized. `Casks/deepzora.rb` will be created by the first stable
Deepzora release. Until then, the CLI is not installable from this tap.

tap 已初始化。首次正式稳定发布会自动创建 `Casks/deepzora.rb`；在此之前无法通过
这个 tap 安装 CLI。

After the first stable release / 首次稳定发布后：

```sh
brew tap SivanCola/deepzora
brew install --cask SivanCola/deepzora/deepzora
```

## Publishing / 发布维护

Deepzora's release workflows update `Casks/deepzora.rb` on this repository's `main`
branch. Store the dedicated `HOMEBREW_TAP_TOKEN` secret in `SivanCola/deepzora`.
The token needs Contents read/write access to only this tap and the automatically
required Metadata read access. See the
[release setup guide](https://github.com/SivanCola/deepzora/blob/main/docs/DEEPZORA_INDEPENDENCE.md#homebrew-token--homebrew-专用-token).

Deepzora 发布工作流更新本仓库的 `main` 分支。专用 Token 只授权本 tap 的 Contents
读写权限，保存在 `SivanCola/deepzora` 的 Actions Secret 中；过期前更换。

The tap is MIT licensed. Deepzora retains its original license and authorship in
the application repository's LICENSE and NOTICE files.

tap 采用 MIT 许可证；应用本身的原许可证及作者信息保留在主仓库的 LICENSE 和 NOTICE 中。
