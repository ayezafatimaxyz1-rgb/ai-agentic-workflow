# VANTOR: The Design Package

The single deliverable of the Creative Director's Loop. Written before any generation.
Every line of copy below ships verbatim. Band ranges are starting points, validated by
the flick test.

Tier 1, one continuous 6 second shot.

## 1. The brand premise

**Everything comes to a point.**

VANTOR's mark is a V: two edges that descend and meet. The name comes from avant, from
moving forward, and the brand's own story calls it "a bold, decisive edge." So the site
is built as a descent that resolves. The camera descends the jacket and comes to rest.
The V draws itself down both sides of the screen and meets at its point at the exact
moment the film settles. The page descends through four sections to one call to action.
Mark, film and structure are the same gesture.

Every section serves this. Anything that does not, does not ship.

## 2. The palette as CSS tokens

Sampled from LOGO.png, STORE.png, HARDWARE DETAILS.png and PACKAGING.png. The bronze
was consistent across all four: highlight near #F0C08C, mid near #9A6840, deep near
#6A4527. Canvas is warm near black, never pure black.

```css
:root{
  --canvas:#0B0907;         /* page background, warm tinted toward the store's grade */
  --canvas-deep:#060504;    /* the recessed lane behind the hero stage */
  --panel:#14100C;          /* cards and raised surfaces */
  --accent:#C08A52;         /* the CTA and rare emphasis, the bronze mid to highlight */
  --accent-hover:#E0AE77;
  --accent-muted:#6A4527;   /* whisper level: borders, glows, the V's undrawn stroke */
  --text-primary:#F2E8DA;   /* warm off white */
  --text-secondary:#A79684;
  --hairline:#241C15;       /* decorative rules only, never an interactive border */
  --border-interactive:#4A3826;  /* interactive borders, which need their own stronger value */
}
```

## 3. The type trio

- **Display: Cinzel**, weights 400 and 600. A classical roman serif with cut serifs, the
  closest honest match on Google Fonts to VANTOR's own wordmark. Set in caps with generous
  tracking, as the wordmark is.
- **Body: Jost**, weights 300 and 400. A quiet geometric sans that reads expensive next to
  a classical serif and stays out of the way.
- **Mono: IBM Plex Mono**, weight 300. Small labels, the size ladder, the care line, section
  numerals. Letterspaced and tiny.

Neither Inter nor Roboto appears anywhere.

## 4. The film

**Subject:** Product 7, the brown cafe racer with antique brass hardware.

Revised from the black flight bomber once the brass jacket arrived, and the reason is
brand coherence. VANTOR's accent is aged bronze: the logo, the hang tags, the foiled box,
the storefront signage and the engraved hardware shot are all that one colour. This is the
only jacket in the range whose hardware is that exact finish, so the film and the page end
up in one palette rather than two. Three practical reasons on top of the brand one: brown
separates from a black room, where a black jacket with blacked out hardware risks reading
as a silhouette; the brass gives the descending camera something to catch light on, which
is what keeps a locked path from reading as dead footage; and its grain is lightly
distressed, which reads as real hide faster than a uniform surface does.

The Vintage Bomber was the closest rival and lost only on hardware, its zip being silver.
It earns the proof section instead, where its patina does more work than it would as a
silhouette in a dark room.

The black flight bomber leads the range section instead, where the white studio background
suits it.

**World:** the VANTOR store's own room, taken from STORE.png. Dark stone, deep shadow, one
warm bronze light from above.

**Start frame (16:9, 2k):** the jacket hangs on a slim bronze rail in a dark stone room.
The camera sits high and close on the band collar and the upper chest. The distressed grain
reads large. The antique brass throat snaps and the top of the brass zip catch one warm
edge of light. The stone wall behind recedes into shadow. The world fills the frame edge
to edge, with the calm falloff of shadow to the left and right of the jacket where the
captions will live.

**Motion:** one continuous shot, no cuts. The camera descends straight down the front of
the jacket, past the collar tab, down the brass zip line, past the twin zip chest pockets,
easing back as it falls so more of the jacket enters frame. It passes through the soft edge
of the light beam on the way, a brief bloom across the lens. The leather stays alive,
shifting very slightly as though the air moved. Dust drifts through the beam throughout.

**The ending, planned first:** the whole jacket hanging centred and still, warm light raking
from the upper left, the brass catching at the collar and the hem, deep shadow around it,
generous empty margin above and below the garment so the fixed header never crowds the
shoulders and a cover crop on a short window never eats the hem. Verified with the header
mocked over it at a wide window and a short one before approval.

**Laws check:** descends, so down reads as down (1). One subject, one motion, no cuts (2).
Path locked, leather and dust alive (3). Ending written first and composed (4). Leather is
a forgiving subject with no anatomy (5). Vertical axis (6). Action lane centre, captions
flanking (7). The light beam edge is the lens moment (8). The mark is on the hardware and
the ending lands close enough to read it (9). Legibility system below (10). Bands paced in
vh (11). No text, no logos, no lettering written into every prompt (12).

## 5. The band map

Hero height 700vh, so the scroll range is 600vh. Ramps compute to 0.02 of progress, which
is 12vh here.

| Band | Range (starting point) | Footage moment | Copy (verbatim) | Entrance |
|---|---|---|---|---|
| 1 | 0.00 to 0.20 | High and close on the band collar, grain large, brass catching one edge | **"Nobody grows into bold."** / "You put it on." | Drift-down, echoing the camera's fall. Opens settled via the one time load ramp. |
| 2 | 0.25 to 0.45 | Descending the brass zip line, grain filling the frame | **"Grain you can read across a room."** / "Genuine leather. Heavy hand. No plastic shine." | Grid snap-align, characters sliding into place in reading order, echoing the zip teeth passing |
| 3 | 0.50 to 0.68 | Past the twin zip pockets, camera easing back, dust in the beam | **"The mark is small on purpose."** / "One V, on the snap. That is the whole logo." | Blur-to-sharp, echoing the beam's bloom clearing |
| 4 | 0.74 to 1.00 | The jacket at rest, whole, lit from upper left | **"Built for a bolder you."** / "Eleven jackets. One mark. Made responsibly." / CTA: **"See the range"** | Word-by-word rise into a staged settle: headline, then subline, then the CTA row |

Band 2 is placed deliberately. It answers the objection buyers named first, that the
leather is fake, at the exact moment the footage is showing them the grain.

## 6. The static-hero copy block

For phones, portrait tablets, landscape phones and reduced motion. Composed over the
ending frame.

- Headline: **"Built for a bolder you."**
- Subline: **"Eleven jackets. One mark. Genuine leather, made responsibly."**
- CTA: **"See the range"**

## 7. The below-fold outline

Every section funnels to the single anchor `#enquire`.

**a. The range**
- Kicker: `01 / THE RANGE`
- Headline: **"Eleven jackets. No filler."**
- Lede: "Every one of them is lined, finished with the same mark, and cut to be worn hard."
- Eleven cards in a three column grid, each using the owner's real photographs, no generated
  stand ins. Lazy loaded below the first row:
  - **The Cafe Racer** / "Brown. Band collar, twin zip chest pockets, antique brass throughout."
  - **The Vintage Bomber** / "Antique brown. Mottled patina, band collar, flap patch pockets."
  - **The Flight Bomber** / "Black. Pebbled grain, flap chest pockets, blacked out hardware."
  - **The Trucker** / "Black. Cropped, patch pockets, V snaps down the placket."
  - **The Crop Bomber** / "Black. Crinkled grain, elasticated cuffs and hem."
  - **The Bomber** / "Brown. Spread collar, two way zip, VANTOR on the pull."
  - **The Bomber, Oxblood** / "Burgundy. Spread collar, centre zip, V snaps at the cuff."
  - **The Moto** / "Brown. Notch lapels, snap down, zip chest pocket."
  - **The Moto, Olive** / "Olive. Asymmetric zip, epaulettes, elasticated hem."
  - **The Cafe Racer, Bone** / "Cream. Band collar, twin snaps, gunmetal hardware."
  - **The Field Bomber** / "Stone. Band collar, flap chest pockets, snap placket over the zip."
- Every card gets an image, all eleven treated identically. A card without one would read as
  a hole to a first time visitor.

**b. The make** (the proof, answering objection one)
- Kicker: `02 / THE MAKE`
- Headline: **"How to tell it is real."**
- Lede: "Four things a good jacket does that a cheap one cannot. Check ours against all four."
- Four items, each with its own image, equal treatment:
  - **"It has a grain, not a pattern."** / "Real hide repeats nothing. Hold two panels side by side and they will not match."
  - **"It drinks water."** / "A drop sinks in and darkens. On plastic it sits there and beads."
  - **"It has weight."** / "You feel it on your shoulders the first time you put it on. That is the point."
  - **"It smells like leather."** / "There is no substitute for this one and everybody knows it."
- Section image: the owner's HARDWARE DETAILS photograph for the hardware claim, and the
  Vintage Bomber's mottled patina panel for the grain claim. That jacket is the strongest
  visual proof in the whole range that this leather ages rather than degrades, which is the
  single thing premium buyers said they want most.

**c. The moment** (the one interactive element)
- Kicker: `03`
- Headline: **"Everything comes to a point."**
- Instruction: **"Press and hold."**
- The visitor presses and holds. A line draws downward from the top of the panel, splits
  into the two strokes of the V, and the strokes travel down and meet at the point. As
  they meet, the brand story lights up in sequence beneath. Releasing early eases the
  progress back down, it never snaps. Reduced motion gets the finished state with no hold.
- The copy that lights up, from the owner's own brand story, verbatim:
  **"VANTOR is inspired by the spirit of moving forward, drawn from the idea of avant and strengthened by a bold, decisive edge."**
  **"Crafted for those who refuse to blend in."**
  **"More than a jacket. A state of mind."**

**d. The box** (the arrival)
- Kicker: `04 / THE ARRIVAL`
- Headline: **"It shows up like it costs what it costs."**
- Lede: "Foiled box, tissue, a card. Nothing plastic in the whole package."
- Uses the owner's PACKAGING.png.

**e. Fit and returns** (answering objection two, the real fear)
- Kicker: `05 / FIT`
- Headline: **"Cut oversized. Sized honestly."**
- Body: "Every jacket here is cut oversized on purpose, so take your normal size unless you want it roomier still. The size ladder runs S through XXL."
- A size ladder rendered in mono type.

**f. FAQ** (the remaining objections, in the buyers' own words)
- Kicker: `06`
- Headline: **"The questions people actually ask."**
- **"Is this real leather or is it PU?"** / "Genuine leather, with a polyester lining. The care tag on every jacket says so, and so does the grain."
- **"Will it crack in two years?"** / "Cheap bonded leather cracks because it is ground up scrap held together with glue. This is hide. Keep it out of direct heat, clean it professionally, and it outlives the trend that sold it to you."
- **"It looks stiff. Does it soften?"** / "Yes. The first few wears are the stiffest it will ever be, and it moulds to your shoulders from there."
- **"What if it does not fit?"** / "Tell us and we sort it out. No restocking fee."
- **"Why is it this price?"** / "Hide, hardware and lining, in that order. Nothing here is decoration."

**g. The call to action**
- Kicker: `07`
- Headline: **"Built for a bolder you."**
- Lede: "Tell us which one caught your eye and we will come back to you."
- Form: Name, Email, Which jacket (a select listing all eleven), Message.
- Button: **"Send it"**
- Success state: **"Got it. We will come back to you shortly."**
- **Form handling:** a JavaScript success state, because there is no backend on a static
  site and no business inbox was supplied. The submission goes nowhere. This is marked in
  the HTML with a clearly labelled comment so it can be switched to a mailto link or a
  Formspree endpoint in one line the moment an address exists. The owner is told this
  plainly.

**h. Footer**
- The V mark, the wordmark, "BUILT FOR A BOLDER YOU", vantorworld.com, the care line
  "Genuine leather. Lining 100% polyester. Professional leather clean only. Made responsibly."
- No fictional-brand disclosure, because VANTOR is the owner's real brand.

## 8. The vector layer plan

- **The signature: the descending V.** Two SVG strokes, fixed to the hero stage, drawing
  downward from the top corners as hero progress rises and meeting at the point at exactly
  progress 1.0, the instant the film rests. Drawn by hand as a path, stroked in
  `--accent-muted` at whisper level, with the meeting point flaring briefly to `--accent`.
  Remove it and the page loses its spine, which is the test of a real signature.
- **The tissue motif.** The repeating V from the owner's wrapping tissue, redrawn as an SVG
  pattern, used at about 3 percent opacity as the fixed background environment layer behind
  the whole page, drifting on a 90 second cycle so scrolling feels like moving through a room.
- **Section rules.** Short bronze hairlines that draw themselves left to right on entry.
- **Particles.** Dust motes at whisper level in the hero and the make section only, echoing
  the beam in the footage.
- All of it honours reduced motion: final states shown, drives stopped, and un-pinned again
  if the visitor flips reduced motion back off.

## 9. The engineering list

The full standard in `.claude/skills/10k-websites/references/scrub-pipeline.md`, named here
so the build cannot half remember it: the Blob fetch with the poster winning the bandwidth
race and a loading ring with a watchdog if the file exceeds about 8MB; the dt-normalised
lerp in a rAF loop that rests on convergence and off screen; gated seeks with the error
handler deadlock escape; delta-gated DOM writes; band pacing validated by the flick test at
120, 240 and 360px; the four layer legibility system audited at 3.5:1 on each band's worst
frame; one entrance per band echoing the footage, transform and opacity only, reversible;
the five static hero gates identical character for character in CSS and JS and re-evaluated
live; complete and beautiful without the video; plus the whole-site-animated standard and
the quality floor.

## 10. The copy gate

Every viewer-facing line above ships verbatim. The built page must pass the Phase 9 grep
gate with zero em dashes and zero stock words, plus the body copy sweep for AI tells,
before anyone sees it.

Deliberate devices in this package that stay: the four-item parallel lists in The Make and
The Range, and the staccato product descriptions. These were chosen for this brand on
purpose. The sweep hunts what drifted in uninvited, not these.

## 11. Declared deviations

- **The banned look, taken deliberately.** The standard warns off near black with a warm
  amber accent and a high contrast serif, because it is the default reach whenever anyone
  says dark or cinematic. VANTOR's actual logo, hang tags, care tag, packaging and
  storefront are exactly that. The carve-out applies: it is the subject's own material
  world, not a default. Earned by sampling the tones from the owner's own files rather than
  inventing them, by inventing the descending V signature, and by refusing the stock dark
  template layout. No two adjacent sections share a skeleton.
- **Hero height 700vh rather than the 400vh Tier 1 default**, so four beats each get a real
  plateau rather than three cramped ones.

## 12. Open assumptions, flagged for the owner

1. **Hardware finish.** The brand kit is aged bronze, all four products are silver or
   blacked out. The site commits to bronze as the brand colour for type, rules and the V,
   and leaves the product photographs exactly as shot. Nothing is recoloured or faked.
2. **Price.** No price was supplied, so no price appears. The call to action is an enquiry
   rather than a checkout.
3. **Genuine leather.** The care tag's wording is used as supplied. Worth noting to the
   owner that this exact phrase is the one premium buyers distrust, and naming the hide
   would convert better.
