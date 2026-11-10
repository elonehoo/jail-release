# Jail 更新发布

这个仓库只用来发布 Jail 的安装包。源码在 [elonehoo/claude-cage](https://github.com/elonehoo/claude-cage)。

应用检查更新时读取：

`https://api.github.com/repos/elonehoo/jail-release/releases`

仓库保持公开，因为检查更新不携带登录凭据。

每个版本使用 `v` 加语义化版本作为标签，例如 `v0.1.8`。一次发布至少包含：

- `Cage-<版本>-macos-arm64.dmg`
- `SHA256SUMS`

macOS 安装包必须使用 Developer ID 签名并完成公证。磁盘镜像里的应用是 `Jail.app`。临时签名的开发包不能进入这条更新通道。
