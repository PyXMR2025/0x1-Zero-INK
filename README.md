# 0x1 Zero INK

> [Jackie](https://github.com/PyXMR2025)'s personal blog, built with modern static site generators and hosted on GitHub Pages and Cloudflare.
> **Website**: [blog.zjackie.ink](https://blog.zjackie.ink)

[![License: Code MIT](https://img.shields.io/badge/License-Code%20MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![License: Content CC BY-NC-SA 4.0](https://img.shields.io/badge/License-Content%20CC%20BY--NC--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-sa/4.0/)
[![Deploy Status](https://github.com/PyXMR2025/0x1-Zero-INK/actions/workflows/deploy.yml/badge.svg)](https://github.com/PyXMR2025/0x1-Zero-INK/actions)

## Tech Stack

- **Core**: [Zensical](https://zensical.org/) / [MkDocs](https://www.mkdocs.org/) (Next-gen Static Site Generator)
- **Theme**: Material for MkDocs
- **Language**: Python
- **CI/CD**: GitHub Actions
- **Hosting**: GitHub Pages & Cloudflare

## Project Structure

*(Note: This is a simplified view of the core directories.)*

```text
.
├── .github/
│   └── workflows/
│       └── deploy.yml      # GitHub Actions workflow for automated deployment
├── docs/                   # All Markdown blog posts and assets
│   ├── index.md            # Homepage
│   └── blog/               # Blog posts directory
├── zensical.toml           # Site configuration
├── requirements.txt        # Python dependencies
└── README.md               # You are here!
```

## Local Development

To run this blog locally, you need **Python 3.8+** installed.

1. **Clone the repository**:
   ```bash
   git clone https://github.com/PyXMR2025/0x1-Zero-INK.git
   cd 0x1-Zero-INK
   ```

2. **Set up a virtual environment** *(Recommended, do not commit `.venv` to Git)*:
   ```bash
   python3 -m venv .venv
   source .venv/bin/activate  # On Windows: .venv\Scripts\activate
   ```

3. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   # Or install directly: pip install zensical mkdocs-material
   ```

4. **Start the local preview server**:
   ```bash
   zensical serve
   # Or fallback to: mkdocs serve
   ```
   Open your browser and navigate to `http://127.0.0.1:8000`.

## Automated Deployment

This repository uses **GitHub Actions** for continuous deployment.
Whenever new commits are pushed to the `main` branch, the workflow in `.github/workflows/deploy.yml` automatically:
1. Checks out the code.
2. Sets up the Python environment.
3. Builds the static site using Zensical/MkDocs.
4. Deploys the generated `site/` directory to GitHub Pages.

*No manual deployment steps are required!*

## Contributing & i18n (Internationalization)

Contributions are always welcome! If you'd like to help translate this blog into your native language or improve existing translations, please follow these simple steps:

1. **Locate the Language Directory**: Check the `docs/` directory. If your language folder (e.g., `docs/zh/`, `docs/ja/`) already exists, you can directly translate or update the Markdown files within it.
2. **Add a New Language**: If your language is not yet supported, create a new folder using the standard [ISO 639-1 language code](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes) (e.g., `docs/fr/` for French). Mirror the structure of the default language directory and translate the content.
3. **Update Configuration**: If you are adding a completely new language, please also update the `mkdocs.yml` (or `zensical.toml`) to register the new locale in the `i18n` plugin settings.
4. **Submit a Pull Request**: Fork the repository, commit your changes, and open a Pull Request. Please include a brief description of the language and files you've worked on.

> **Tip**: While AI translation tools are helpful, please ensure the final content is reviewed by a human for accuracy, context, and natural phrasing.

## Support & Donate

If you find this blog helpful or enjoy the content, consider supporting my work! Your contributions help keep the infrastructure running and fuel future open-source projects.

**Bitcoin (BTC)**:

```text
bc1pyhjz2ene2m88pwv8k4v3ql72c4pqqrvdvq8w75x2f0whzhf699aq2pl7yk
```

<details>
<summary><b>PGP Signature Verification</b> (Click to expand)</summary>
<br>
<em>The donation address above is cryptographically signed to prevent tampering. You can verify this signature using my public key.</em>
<br><br>

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

## License

This project uses a **Dual License** approach to protect both the code and the content:

- **Code & Infrastructure**: The build scripts, configuration files, and custom code are licensed under the [MIT License](LICENSE).
- **Blog Content**: All original blog posts, articles, and media content (located in the `/docs` directory) are licensed under the [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License (CC BY-NC-SA 4.0)](https://creativecommons.org/licenses/by-nc-sa/4.0/).

---

Made with ❤️ by [Jackie](https://github.com/PyXMR2025)
