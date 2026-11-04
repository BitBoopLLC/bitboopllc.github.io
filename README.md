# Bit Boop LLC

The Bit Boop LLC homepage. A responsive static site using the official Bit Boop brand kit, with no JavaScript or build dependencies.

## Preview locally

From this directory, run:

```sh
python3 -m http.server 8000 --bind 127.0.0.1
```

Open http://127.0.0.1:8000. Stop the server with Control-C.

## Publish with GitHub Pages

1. In the GitHub repository, open **Settings → Pages**.
2. Under **Build and deployment**, set **Source** to **GitHub Actions**.
3. Push the site files and `.github/workflows/pages.yml` to `main`.

The workflow publishes the static site to **https://bitboopllc.github.io/** on every push to `main`. It can also be started manually from the Actions tab. No deployment secrets are needed. Any organization policy or environment protection that requires approval still applies.

The workflow copies only public site files into `_site`; repository documentation and workflow files are not published. The initial deployment can only be verified after pushing and enabling Pages.

## Editing

- `index.html`: page content, metadata, and links.
- `styles.css`: layout, responsive styles, and brand colors.
- `assets/`: official SVG marks and self-hosted Space Grotesk font.
- Root icons, `site.webmanifest`, and `og-image.png`: supplied brand web assets.

Brand assets were copied from `../bit-boop-branding/`. Space Grotesk is distributed under the SIL Open Font License included in `assets/fonts/SpaceGrotesk-OFL.txt`.

The site currently uses the GitHub Pages URL. When connecting a custom domain, update the canonical site URLs in the Open Graph metadata, `robots.txt`, and `sitemap.xml`, and configure the domain in GitHub Pages. Add an HTML canonical link then if desired. No custom domain or contact email is assumed.
