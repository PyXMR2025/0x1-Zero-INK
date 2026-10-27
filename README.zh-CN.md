# 0x1 ZeroINK

> Jackie 的个人博客，基于现代静态站点生成器构建，并托管于 GitHub Pages 与 Cloudflare。

**URL**: [https://blog.zjackie.ink](https://blog.zjackie.ink)

## 本地开发

要在本地运行此博客，请确保您的环境中已安装 **Python 3.8 或更高版本**。

1. **克隆仓库**：
   ```bash
   git clone https://github.com/PyXMR2025/0x1-ZeroINK.git
   cd 0x1-ZeroINK
   ```

2. **配置虚拟环境**（强烈建议，请勿将 `.venv` 目录提交至 Git）：
   ```bash
   python3 -m venv .venv
   source .venv/bin/activate  # Windows 用户请使用: .venv\Scripts\activate
   ```

3. **安装依赖**：
   ```bash
   pip install -r requirements.txt
   ```

4. **启动本地预览服务**：
   ```bash
   zensical serve
   ```
   命令执行后，请在浏览器中访问 `http://127.0.0.1:8000` 即可查看博客效果。

## 贡献与国际化 (i18n)

我们随时欢迎社区贡献！如果您希望将此博客翻译成您的母语，或改进现有的翻译内容，请遵循以下简单步骤：

1. **定位语言目录**：检查 `docs/` 目录。如果目标语言的文件夹（例如 `docs/zh/`、`docs/ja/`）已存在，您可以直接在其中翻译或更新对应的 Markdown 文件。
2. **添加新语言**：如果尚未支持您的语言，请使用标准的 [ISO 639-1 语言代码](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes)创建一个新文件夹（例如法语为 `docs/fr/`）。请参照默认语言目录的结构，并翻译其中的内容。
3. **更新配置文件**：若添加了全新的语言，请同步修改 `zensical.toml` 文件，在 `i18n` 插件的设置中注册该新语言。
4. **提交 Pull Request**：Fork 本仓库，提交您的更改并发起 Pull Request。请在 PR 描述中简要说明您翻译的语言及涉及的文件。

> **提示**：虽然 AI 翻译工具能提供很大帮助，但请务必进行**人工校对**，以确保译文在准确性、语境和表达习惯上自然流畅。

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
- **博客内容**：所有原创博客文章、文本及媒体内容（位于 `/docs` 目录下）均采用 [知识共享 署名-相同方式共享 4.0 国际许可协议 (CC BY-SA 4.0)](https://creativecommons.org/licenses/by-sa/4.0/)。

---

Made with ❤️ by Jackie
