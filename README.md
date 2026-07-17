# Hung Luong — GitHub Pages website

This folder is the standalone static version of Hung Luong’s academic website for `https://hqluong.github.io/`. It includes the corrected responsive layout, headshot, academic CV, favicon, and social-sharing card. It does not require WordPress, Node.js, or a build step.

## Publish on GitHub Pages

1. Open the existing `hqluong/hqluong.github.io` repository.
2. Replace its current website files with everything in this folder, including the hidden `.nojekyll` file.
3. In the repository, open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select the `main` branch and the `/ (root)` folder, then save.

GitHub will publish the website at `https://hqluong.github.io/`. All internal website links use relative paths, so the headshot, CV, social card, and stylesheet remain portable.

## Social-sharing URL

The social-card image is included at `assets/social-card.png`. The `og:image` and `twitter:image` values in `index.html` are already configured with the complete public URL:

```html
<meta property="og:image" content="https://hqluong.github.io/assets/social-card.png">
<meta name="twitter:image" content="https://hqluong.github.io/assets/social-card.png">
```

## Included files

- `index.html` — complete one-page academic website
- `styles.css` — responsive design and mobile layout
- `assets/hung-luong-headshot.jpg` — headshot used in the hero section
- `assets/Hung_Luong_Academic_CV.pdf` — downloadable academic CV
- `assets/social-card.png` — social-sharing image
- `assets/favicon.svg` — browser icon
- `.nojekyll` — tells GitHub Pages to serve the files directly

The existing WordPress site at `hungqluong.com` is unaffected. Do not add a GitHub Pages custom-domain file unless you intend to move that domain away from WordPress.
