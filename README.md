# Ey Up, Ahoj! 🫖

A daft but genuinely useful **Yorkshire ⇄ Czech phrasebook**.

Forty hand-picked phrases, each with its meaning and a cheeky translator's note. It works both ways: Yorkshire to Czech for Tykes let loose in Prague, and Czech to Yorkshire for Czechs let loose in Leeds.

## Features

- Both directions, with one-tap **⇄ Swap**
- Meaning plus a funny note for every phrase
- Search by keyword ("tea", "pub", "pivo", "rain"…)
- **Another one** button for a random phrase
- **🔊 Say it** reads phrases aloud using your browser's built-in voices, including Czech where your device has a Czech voice
- Light and dark mode, works on phones
- One self-contained HTML file: no login, no backend, no build step

## Try it

Live at: `https://<your-username>.github.io/yorkshire-czech-phrasebook/`

Or download `index.html` and open it in any browser.

## Deploy your own (GitHub Pages)

1. Push this repo to GitHub.
2. Go to **Settings → Pages**.
3. Under **Build and deployment**, set Source to **Deploy from a branch**, branch **main**, folder **/ (root)**, then **Save**.
4. After a minute or so, your site is live at the URL above.

## Adding phrases

All phrases live in two arrays near the top of the `<script>` in `index.html`: `YK` (Yorkshire → Czech) and `CZ` (Czech → Yorkshire). Each entry looks like this:

```js
["Put t’kettle on.", "Postav vodu na čaj.", "Put the kettle on.", "The funny note goes here.", "search words here"]
```

The fields are: original phrase, translation, plain-English meaning, note, and search tags.

## Disclaimer

Translations are lovingly mangled. Do not use for legal documents, wedding vows or ordering at a Michelin-star restaurant. Flat caps not included.

## Licence

MIT. See [LICENSE](LICENSE).
