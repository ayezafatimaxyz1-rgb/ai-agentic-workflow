# VANTOR

A scroll driven site for VANTOR. Plain HTML, CSS and vanilla JavaScript.
No framework, no build step, no npm. `index.html` plus `assets/`.

## Look at it locally

Double clicking `index.html` works, but you will see the **still image hero**
rather than the scrolling film. That is not a fault. Browsers block `fetch` on
`file://` addresses, so the video loader falls back to the still by design.

For the real thing, serve the folder and open the link in a browser:

```
npx http-server        # or:  python3 -m http.server
```

Then open the localhost address it prints.

## Changing things

**Prices.** Open `index.html` and find `var PRICES`. The eleven prices there are
placeholders in AED, set by eye against what comparable premium jackets sell for,
so the page had real numbers to argue around. Change any of them and that card
updates. Leave one empty and it shows no price. `CURRENCY` just above changes the
prefix if you sell in something else.

**Where the form goes.** Find `ACTION_EMAIL` and `ACTION_POST`, near the bottom.
Set `ACTION_EMAIL` to an inbox and the send button opens the visitor's email app
addressed to you. Set `ACTION_POST` to a Formspree endpoint and messages arrive
in that inbox instead. Leave both empty, as they are now, and the form shows its
thank you and the message goes nowhere.

**Before putting it online.** Find the `<!-- DEPLOY STEP -->` comment in the head
and put the real address into `og:url` and `og:image`, or link previews will
point at the wrong place.

## What is in assets

- `room/` five photographs of the same wardrobe room at five points in its build,
  cross faded by scroll so the wardrobe assembles itself. The camera never moved
  between them, which is the whole reason the dissolve reads as one room rather
  than five.
- `spin/<jacket>/` each jacket's angles, ordered into a turn and cut out of their
  studio background. Frame 01 is the front, and it doubles as the card image.
- `hero-scrub.mp4` and `.webm` the six second film, on the cafe racer's page.
  Two encodes because Safari needs H.264 and some Chromium builds cannot decode
  it at all.
- `hero-ending.jpg` its resting frame, used for the link preview
- `brand/` the storefront and the packaging photographs
- `fonts/` Cinzel, Jost and IBM Plex Mono, served from here so the page depends
  on no third party
