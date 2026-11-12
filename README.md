# Craft Apps — web launcher

https://zhvial.github.io/

A small launcher (`index.html`) for unmodified web builds of three open-source apps, each
taken from its official GitHub release and served by GitHub Pages:

| App | Folder | Version | Source zip (SHA256 checked against the release's `SHA256SUMS.txt`) |
|---|---|---|---|
| CADCraft | [`cadcraft/`](cadcraft/) | 0.20.1 | [storytold/cadcraft v0.20.1](https://github.com/storytold/cadcraft/releases/tag/v0.20.1) `cadcraft-web-0.20.1.zip` `300e870c50b66d371055915ba95e3ddbfd4c45431466d5214743b5dcab95a0e1` |
| PhotoCraft | [`photocraft/`](photocraft/) | 0.23.1 | [storytold/photocraft v0.23.1](https://github.com/storytold/photocraft/releases/tag/v0.23.1) `photocraft-web-0.23.1.zip` `3a498eb517bca6cec89f9c6b1fc6448269a05428c8a3a4637c16817da157f03c` |
| SolidCraft | [`solidcraft/`](solidcraft/) | 0.30.1 | [tangency-labs/solidcraft v0.30.1](https://github.com/tangency-labs/solidcraft/releases/tag/v0.30.1) `solidcraft-web-0.30.1.zip` `acaa73a5638206cf123c56b4c0a5113c83a8bf0149dee6a66b929b00fe444403` |

The apps run entirely in the browser (WebAssembly); there is no server-side code.
PhotoCraft (0.21.0 – 0.23.1): `photocraft/app/snippets/eframe-d31a8450ea12dfc1/inline0.js` is added as a copy of
`photocraft/snippets/...` — the release zip lacks it, though `app/photocraft-web.js` imports it from there
(without it the app hangs on "Loading PhotoCraft…"). Drop the copy once a release ships it.

Each folder keeps the app's own `LICENSE-APACHE`, `LICENSE-MIT` and `NOTICE`.
Icons in `icons/` come from the apps' repositories under the same licences.

To update an app: replace the contents of its folder with the new release zip's site
folder, then update the version in `index.html` (`APPS`) and in the table above.
