# CLOSET — 发布产物

这个仓库**只放安装包与自动更新清单，不放源码**。

- `CLOSET_<版本>_aarch64.dmg` —— macOS（Apple 芯片）安装包。
  **第一次打开要右键点图标选「打开」**，双击会被系统拦下；应用没有经过 Apple 公证。
- `CLOSET.app.tar.gz` + `.sig` —— 应用内「检查更新」用的更新包与签名。
- `latest.json` —— 更新清单。应用读的是
  `https://github.com/jx921170819-dev/closet-releases/releases/latest/download/latest.json`，
  所以**每一版都要重新上传这个文件**。

源码在另一个私有仓库里。这个仓库之所以是公开的，是因为应用要匿名读取它的 release ——
把访问私有仓的 token 打进应用等于把源码读权限发给每一个用户。
