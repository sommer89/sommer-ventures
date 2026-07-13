# sommerventures.dk

The company website for **Sommer Ventures ApS**, an independent investment and holding company in
Denmark. Static HTML, no build step, no dependencies — served from GitHub Pages.

<https://sommerventures.dk>

## Structure

```
index.html                      the company
apps/index.html                 the software we build
apps/football-owner/            Football Owner — description + support
apps/football-owner/privacy/    Football Owner — privacy policy
assets/styles.css               all styling, light + dark
assets/apps/                    app icons
404.html                        fallback page
CNAME                           custom domain
```

Tukd is not hosted here — it has its own site at <https://tukd.app>.

## Local preview

```sh
python3 -m http.server 8000
# open http://localhost:8000
```

## Adding an app

If the app has its own site, add a panel to `index.html` and `apps/index.html` pointing at it.
Otherwise copy `apps/football-owner/` and write the two pages: a description with a support contact,
and a privacy policy.

One privacy policy per app, at one URL. Two copies in two places drift apart.

---

© 2026 Sommer Ventures ApS · CVR 46590538
