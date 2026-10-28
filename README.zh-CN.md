# 0x1 ZeroINK

> Jackie 的个人博客，基于 [Hugo](https://gohugo.io/) + [PaperMod](https://github.com/adityatelange/hugo-PaperMod) 主题构建，并托管于 GitHub Pages 与 Cloudflare。

**URL**: [https://blog.zjackie.ink](https://blog.zjackie.ink)

## 本地开发

要在本地运行此博客，请确保您的环境中已安装 **Hugo（Extended 版本）**。

1. **克隆仓库**（主题为 Git submodule）：
   ```bash
   git clone --recurse-submodules https://github.com/PyXMR2025/0x1-ZeroINK.git
   cd 0x1-ZeroINK
   ```
   如果克隆时未包含 submodule：
   ```bash
   git submodule update --init --recursive
   ```

2. **启动本地预览服务**：
   ```bash
   hugo server -D
   ```
   命令执行后，请在浏览器中访问 `http://localhost:1313` 即可查看博客效果。

3. **创建新文章**：
   ```bash
   hugo new content content/posts/my-post.md
   ```
   准备发布时，将文章 Front Matter 中的 `draft` 设为 `false`。

## 部署

每次推送到 `main` 分支都会触发 GitHub Actions：

1. 使用 Hugo 构建站点并发布到 `gh-pages` 分支（通过 [blog.zjackie.ink](https://blog.zjackie.ink) 访问）。
2. 将站点地图 URL 提交至 [IndexNow](https://www.indexnow.org/)，实现快速收录。

## 支持与赞助

如果您觉得这个博客对您有帮助，或者喜欢这里的内容，欢迎考虑支持我的工作！您的赞助将帮助维持基础设施的运转，并为未来的开源项目提供动力。

**比特币 (BTC)**:

```text
bc1pyhjz2ene2m88pwv8k4v3ql72c4pqqrvdvq8w75x2f0whzhf699aq2pl7yk
```

**PGP 签名验证** (点击展开)
<details>
<summary>查看 PGP 签名</summary>

```text
-----BEGIN PGP SIGNED MESSAGE-----
Hash: SHA512

bc1pyhjz2ene2m88pwv8k4v3ql72c4pqqrvdvq8w75x2f0whzhf699aq2pl7yk
-----BEGIN PGP SIGNATURE-----

iHUEARYKAB0WIQQTplea0vauG7PFc++wm9vs48gNGQUCat9xvwAKCRCwm9vs48gN
GdoDAP9Thkjy0HjY+7PIta56ySt4PWXlrzirUlZgdQ8Z42LH8QEAuEIkVX94LiWY
SZY8BGnrKXhNVqjIpQHJ+4mXAYB7IQo=
=eDbG
-----END PGP SIGNATURE-----
```

</details>

**通过 trocador.app 赞助**:

[bc1pyhjz2ene2m88pwv8k4v3ql72c4pqqrvdvq8w75x2f0whzhf699aq2pl7yk](https://trocador.app/anonpay/?ticker_to=btc&network_to=Mainnet&address=bc1pyhjz2ene2m88pwv8k4v3ql72c4pqqrvdvq8w75x2f0whzhf699aq2pl7yk&donation=True&simple_mode=False&amount=0.01&name=Jackie&description=%5B+Jackie+%5D+%211x0%21+%5B+Thanks+%5D&email=pyxmr2025@openenet.cn&bgcolor=00000000&direct=True)

## 开源协议

本项目采用**双重许可 (Dual License)** 策略，以同时保护代码与内容：

- **代码与基础设施**：构建脚本、配置文件及自定义代码均采用 [MIT 许可证](https://opensource.org/licenses/MIT)。
- **博客内容**：所有原创博客文章、文本及媒体内容（位于 `/content` 目录下）均采用 [知识共享 署名-相同方式共享 4.0 国际许可协议 (CC BY-SA 4.0)](https://creativecommons.org/licenses/by-sa/4.0/)。

---

Made with ❤️ by Jackie
