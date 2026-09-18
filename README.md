# myko.n0rdy.foo

One page, no build: `index.html`, the avatar, four product icons, two self-hosted typefaces (Bricolage Grotesque for the page, Caveat for the
footer quote, both SIL OFL, licence in `assets/fonts/OFL.txt`). Served by GitHub Pages from the `main` branch root.

## Deploy

Push to `main`. GitHub Pages publishes the root of the branch.

One-time setup:

1. Repo → Settings → Pages → Source: "Deploy from a branch", branch `main`, folder `/ (root)`.
2. Custom domain: `myko.n0rdy.foo` (the `CNAME` file in the repo keeps it across deploys). Tick "Enforce HTTPS"
   once the certificate is issued.
3. DNS at Porkbun: `CNAME  myko  n0rdy.github.io`.

## Editing

- Links and products are plain HTML in `index.html`.
- The avatar is `assets/img/avatar.svg`; the page background of the avatar is the `rect` fill at the top of the file.
  `avatar-450.png` (Open Graph) and `avatar-180.png` (iOS home screen icon) are rendered from it; re-render both
  after changing the SVG.
