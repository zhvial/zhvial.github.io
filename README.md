# Craft Apps — web launcher

https://zhvial.github.io/

A small launcher (`index.html`) for unmodified web builds of three open-source apps, each
taken from its official GitHub release and served by GitHub Pages:

| App | Folder | Version | Source zip (SHA256 checked against the release's `SHA256SUMS.txt`) |
|---|---|---|---|
| CADCraft | [`cadcraft/`](cadcraft/) | 0.18.0 | [storytold/cadcraft v0.18.0](https://github.com/storytold/cadcraft/releases/tag/v0.18.0) `cadcraft-web-0.18.0.zip` `2440d15ebe28ce0a97f107a860f96d3bc21d98381b9f685676843b876a4d9086` |
| PhotoCraft | [`photocraft/`](photocraft/) | 0.21.0 | [storytold/photocraft v0.21.0](https://github.com/storytold/photocraft/releases/tag/v0.21.0) `photocraft-web-0.21.0.zip` `3cf893112507ac192c921e0223a3bd5404a24b3dcf94e7a37d43f5eba2032286` |
| SolidCraft | [`solidcraft/`](solidcraft/) | 0.30.1 | [tangency-labs/solidcraft v0.30.1](https://github.com/tangency-labs/solidcraft/releases/tag/v0.30.1) `solidcraft-web-0.30.1.zip` `acaa73a5638206cf123c56b4c0a5113c83a8bf0149dee6a66b929b00fe444403` |

The apps run entirely in the browser (WebAssembly); there is no server-side code.
Each folder keeps the app's own `LICENSE-APACHE`, `LICENSE-MIT` and `NOTICE`.
Icons in `icons/` come from the apps' repositories under the same licences.

To update an app: replace the contents of its folder with the new release zip's site
folder, then update the version in `index.html` (`APPS`) and in the table above.
