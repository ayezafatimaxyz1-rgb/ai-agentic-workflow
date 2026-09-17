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

- `hero-scrub.mp4` the scroll film, re-encoded with a keyframe every 8 frames,
  which is what makes scrubbing smooth rather than stuttery
- `hero-poster.jpg` the first frame, shown while the film streams in
- `hero-ending.jpg` the resting frame, reused as a design image
- `products/` the eleven jackets, backgrounds removed so they sit on the dark page
- `brand/` the hardware, packaging and patina photographs
- `fonts/` Cinzel, Jost and IBM Plex Mono, served from here so the page depends
  on no third party
