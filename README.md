# IS-Tech website

Static site for GitHub Pages at **https://istiaq66.github.io/**.

| Path | Purpose |
|---|---|
| `/` | IS-Tech home: list of games |
| `/hex-stack-sort/` | Hex Stack Sort game page (Play listing "website") |
| `/hex-stack-sort/privacy.html` | Privacy policy (Play Console + AdMob) |
| `/app-ads.txt` | AdMob authorized sellers. Must stay at the domain root. |

## Publish

1. On GitHub, create a **public** repo named exactly `Istiaq66.github.io`.
2. Push this folder to it (branch `main`).
3. Repo → Settings → Pages → Source: *Deploy from a branch*, `main` / root.
4. After a minute, check:
   - https://istiaq66.github.io/hex-stack-sort/privacy.html
   - https://istiaq66.github.io/app-ads.txt

## Keep in sync with the app

- Adding analytics (e.g. Firebase), accounts or in-app purchases changes
  what data is collected. **Update `privacy.html`** (and its effective date)
  in the same release.
- The "Get it on Google Play" badges link to
  `https://play.google.com/store/apps/details?id=com.istech.hexstacksort`.
  That page only works once the game is in **production**. On launch day,
  delete the `<span class="store-note">Launching soon...</span>` lines in
  `index.html` and `hex-stack-sort/index.html`, and the "coming soon" line
  in `index.html`.
- AdMob → Apps → app-ads.txt: add `https://istiaq66.github.io` as the
  developer website in Play Console so AdMob can verify `app-ads.txt`.
