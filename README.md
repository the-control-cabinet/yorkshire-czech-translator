# Ey Up! 🫖

A daft but genuinely useful **Yorkshire translator** for **Czech**, **Italian**, **Polish** and **American**.

Pick a language, then go either way: Yorkshire into Czech, Italian, Polish or American for Tykes let loose abroad, or back into Yorkshire for visitors let loose in Leeds. 74 phrases in all, each with its meaning and a cheeky translator’s note.

## Features

- Language picker: 🇨🇿 Čeština, 🇮🇹 Italiano, 🇵🇱 Polski, 🇺🇸 American
- Both directions, with one-tap **⇄ Swap**
- Meaning plus a funny note for every phrase
- Search by keyword (“tea”, “pub”, “rain”…)
- **Another one** button for a random phrase
- **🔊 Say it** plays a recorded Yorkshire clip if there is one, otherwise the browser voice reads a phonetic respelling, then reads the other language
- Link straight to a language: add `#cz`, `#it`, `#pl` or `#us` to the address
- A link to the AI version on claude.ai, which adds free-text translation for anyone signed in to Claude
- Light and dark mode, works on phones
- One self-contained HTML file: no login, no backend, no build step

## Try it

Live at: https://the-control-cabinet.github.io/yorkshire-translator/

## Deploy your own (GitHub Pages)

1. Push this repo to GitHub.
2. Go to **Settings → Pages**.
3. Set Source to **Deploy from a branch**, branch **main**, folder **/ (root)**, then **Save**.

## Adding phrases

All phrases live near the top of the `<script>` in `index.html`.

`YK` holds Yorkshire phrases, with a translation for every language. `n._` is the default note; add `n.cz`, `n.it`, `n.pl` or `n.us` for a language-specific one:

```js
{
  y: "Put t’kettle on.",
  m: "Put the kettle on.",
  tags: "tea kettle drink",
  t: {
    cz: "Postav vodu na čaj.",
    it: "Metti su l’acqua per il tè.",
    pl: "Nastaw wodę na herbatę.",
    us: "Can you start the kettle?"
  },
  n: {
    _: "In Yorkshire, the answer to every crisis.",
    cz: "In Yorkshire, the answer to every crisis. Czechs will offer you a beer instead. Both are correct.",
    it: "Italians will offer you an espresso instead. Accept it and say nowt.",
    us: "Plenty of Americans don’t own a kettle and heat tea in the microwave. Stay calm."
  }
},
```

`REV.cz`, `REV.it`, `REV.pl` and `REV.us` hold phrases going into Yorkshire:

```js
["Dáme si pivo?", "Fancy a pint, owd lad?", "Shall we have a beer?", "The note", "search words"],
```

If you add a new Yorkshire line, add a phonetic respelling for it to the `SAY` list too, so the browser voice sounds closer to Yorkshire.

## Recording proper Yorkshire audio

Browser voices don’t do a Yorkshire accent, so for the real thing record the phrases yourself. Save each one as an MP3 in an `audio` folder in the repo, using the exact filename below. The page plays a recording automatically when it finds one, and falls back to the browser voice for any it can’t find.

| Phrase | Filename |
|---|---|
| Ey up! | `audio/ey-up.mp3` |
| Ow do? | `audio/ow-do.mp3` |
| Ey up love, fancy a brew? | `audio/ey-up-love-fancy-a-brew.mp3` |
| Put t’kettle on. | `audio/put-tkettle-on.mp3` |
| Ah’m fair clemmed. | `audio/ahm-fair-clemmed.mp3` |
| Ah’m off t’pub. | `audio/ahm-off-tpub.mp3` |
| It’s a bit nippy out. | `audio/its-a-bit-nippy-out.mp3` |
| It’s black over Bill’s mother’s. | `audio/its-black-over-bills-mothers.mp3` |
| It’s nobbut a bit o’ drizzle. | `audio/its-nobbut-a-bit-o-drizzle.mp3` |
| Ah’m reet mafted. | `audio/ahm-reet-mafted.mp3` |
| Tha what? | `audio/tha-what.mp3` |
| Ee by gum! | `audio/ee-by-gum.mp3` |
| Gi’ over! | `audio/gi-over.mp3` |
| ’Ear all, see all, say nowt. | `audio/ear-all-see-all-say-nowt.mp3` |
| If tha does owt for nowt, do it for thisen. | `audio/if-tha-does-owt-for-nowt-do-it-for-thisen.mp3` |
| Nowt so queer as folk. | `audio/nowt-so-queer-as-folk.mp3` |
| Shut t’door, were tha born in a barn? | `audio/shut-tdoor-were-tha-born-in-a-barn.mp3` |
| Tha’s a reet mardy bum. | `audio/thas-a-reet-mardy-bum.mp3` |
| Where’s tha bin? | `audio/wheres-tha-bin.mp3` |
| Get thisen ’ome. | `audio/get-thisen-ome.mp3` |
| Ta-ra, love! | `audio/ta-ra-love.mp3` |
| Argy-bargy | `audio/argy-bargy.mp3` |
| Cleveland rocks! | `audio/cleveland-rocks.mp3` |
| The Dude abides. | `audio/the-dude-abides.mp3` |
| So what is it? | `audio/so-what-is-it.mp3` |
| Fancy a pint, owd lad? | `audio/fancy-a-pint-owd-lad.mp3` |
| Get it down thi! | `audio/get-it-down-thi.mp3` |
| Where’s t’nearest boozer? | `audio/wheres-tnearest-boozer.mp3` |
| Get it etten! | `audio/get-it-etten.mp3` |
| Ah couldn’t give a monkey’s. | `audio/ah-couldnt-give-a-monkeys.mp3` |
| It’s reet nithering out there. | `audio/its-reet-nithering-out-there.mp3` |
| It’s siling it dahn. | `audio/its-siling-it-dahn.mp3` |
| Ah’ve not two ha’pennies to rub together. | `audio/ahve-not-two-hapennies-to-rub-together.mp3` |
| Tha gets nowt for nowt. | `audio/tha-gets-nowt-for-nowt.mp3` |
| Them as digs ’oles fer others ends up in one thisen. | `audio/them-as-digs-oles-fer-others-ends-up-in-one-thisen.mp3` |
| Stop faffin’ abaht and spit it out. | `audio/stop-faffin-abaht-and-spit-it-out.mp3` |
| Ah’m reet fed up wi’ it. | `audio/ahm-reet-fed-up-wi-it.mp3` |
| No use mitherin’ now. | `audio/no-use-mitherin-now.mp3` |
| Bloody ’ell! | `audio/bloody-ell.mp3` |
| Sling thi ’ook! | `audio/sling-thi-ook.mp3` |
| That’s champion, that! | `audio/thats-champion-that.mp3` |
| Ey up, ’ow do? | `audio/ey-up-ow-do.mp3` |
| Ey up, love! | `audio/ey-up-love.mp3` |
| Good luck, owd lad! | `audio/good-luck-owd-lad.mp3` |
| What a reet mess! | `audio/what-a-reet-mess.mp3` |
| It costs a bloody fortune. | `audio/it-costs-a-bloody-fortune.mp3` |
| Ah dunno, me. | `audio/ah-dunno-me.mp3` |
| Ah’m champing at t’bit! | `audio/ahm-champing-at-tbit.mp3` |
| Nowt to do wi’ me. | `audio/nowt-to-do-wi-me.mp3` |
| It’s reet nithering! | `audio/its-reet-nithering.mp3` |
| Flippin’ ’eck! | `audio/flippin-eck.mp3` |
| Ey up, you lot! | `audio/ey-up-you-lot.mp3` |
| Ah’m off t’chippy. | `audio/ahm-off-tchippy.mp3` |
| Can ah ’ave a pop? | `audio/can-ah-ave-a-pop.mp3` |
| Where’s t’loo? | `audio/wheres-tloo.mp3` |
| Ah’m jiggered. | `audio/ahm-jiggered.mp3` |
| Can we ’ave t’bill, love? | `audio/can-we-ave-tbill-love.mp3` |
| ’Ow much?! | `audio/ow-much.mp3` |

## Disclaimer

Translations are lovingly mangled. Do not use for legal documents, wedding vows or ordering at a Michelin-star restaurant. Flat caps not included.

## Licence

MIT. See [LICENSE](LICENSE).
