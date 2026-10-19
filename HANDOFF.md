# FleshCuts LLC — handoff at ~60%

**Live:** https://10elizabethbell.github.io/fleshCuts/ · **Repo:** https://github.com/10elizabethbell/fleshCuts · **Built:** 2026-10-19 from Muse brief (run 2026-10-19, Facebook group "Ocean county small businesses and services.")

## What's built
- One page, phone first: hero → Fall cleanups → Cleanup results → snow strip → Snow shoveling → Free estimates (3 steps + form) → "Hi neighbors, I'm Brandon." + close → leaf lawn → footer.
- **World:** his flyer's deep forest green and oat beige, turned into October. The hero is a mown, edged lawn covered in maple, oak and beech leaves.
- **Signature element:** drag (finger or mouse) across the lawn and the leaves blow off, tumble, flip and land; leaves raked off the side drift back down after a few seconds. Until someone touches it, an unseen gust rakes across on its own. Grass tips along the top edge sway and bend away from the pointer, and mown stripes show where the lawn is raked clear. On desktop, the open right side holds a raked leaf pile: a real drag scatters it, and leaves falling back down rebuild it. Leaves are capped so they never fly over the headline or buttons. Drags work up, down and sideways (`touch-action:none` on the lawn only; pull-to-refresh off).
- **Carried through the page:** between the fall and snow sections a winter-sky strip where snow falls and banks up; drag sideways to shovel it and the snow gets thrown aside (an unseen shovel clears a pass every ~9s when idle). Each before/after pair rests on its own strip of leaf lawn, with leaves spilling onto the photo's bottom edge. A last leaf lawn sits above the footer.
- **Contact:** phone number top-right (tap to call). Every text button and service row opens a text to (570) 690-1250 with a pre-filled message naming the service. The estimate form (name, town, services, notes) composes a text and asks people to attach photos, which is his own process ("Call or text … with your town and a few photos"). If the text app doesn't open, it shows the message to copy.
- Real photos ("Before" / "After" labels above each, like his flyer; on a phone, each before and after fit on one screen together): the two before/after pairs from his ad flyer, pulled at full resolution (1631×2048 original) and cropped. Logo from his Facebook profile picture, used large in the About section and as the favicon/home-screen icon.
- Tunables are named at the top of the "Living yard" script: `LEAF_DENSITY`, `LEAF_LEN`, `PUSH_R`, `REGROW`, `IDLE`, `GRAVITY`, `SNOW_FLAKES`.

## Assumptions I made
- **Colors** come from his own flyer (deep green CTA panel, beige and pale-blue cards), not the crayon logo. The leaf amber accent is mine.
- **Voice:** first person as Brandon ("I'm Brandon, your neighbor in Brick"), since he posts that way.
- **Hero line** "Your yard, ready for winter." comes from his caption "get your property ready for winter".
- "I'll price match" / "Competitive prices" / "Free estimates" are his caption's words, reworded.
- "the same way" (care for neighbors' yards like the school grounds) is my framing of his two facts (8+ years, full time in grounds and maintenance for Brick Public Schools).
- Audience treated as general homeowners, not 40+, so the motion is on. Snow-shoveling customers may skew older; if Ellie or Brandon says so, switch to `older-audience.md` (still picture, no drag).
- The Facebook link goes to Brandon's **personal** profile (the brief's fallback; no business page exists).
- **Photos are separate files** in `img/` (WebP, ~60KB each, lazy-loaded), not base64 in the HTML. That's lighter on cellular and caches better. The page HTML itself is ~50KB.
- **World choice:** I picked from 7 candidates by the pitch-site rule (brand + touchable material). Impeccable's seed roll (85bf685e) assigned #6, the township's leaf-pickup notice; I didn't build it because it reads like an official Brick Township notice.

## Placeholders and gaps
- **Licensing/insurance not published.** His flyer prints "Licensed & insured in NJ • EIN: 42-4174060 • General liability insured through Spinnaker Insurance Company". The brief says not to publish it until verified. Once he confirms, it's one line to add under the About paragraph or in the footer.
- **Phone area code 570** (NE Pennsylvania) for a Brick NJ business: used as given; confirm it's his business line.
- **No email** anywhere (none found), so the footer has no email line.
- No hours, no prices, no reviews, no list of towns beyond "Brick and surrounding communities".
- Only 2 before/after pairs, and they aren't shot from the same spot, so I show them side by side, not as a drag slider.
- The logo reads "EST 2019"; I didn't use the year on the page (the caption says 8+ years of experience, which may predate the LLC).

## Questions for the owner
- Can we say "Licensed & insured in NJ" on the site (and should the EIN / insurer be shown)?
- Is (570) 690-1250 the number you want customers to use?
- Which towns do you cover, by name?
- Do you have a Facebook business page, or should the link stay on your personal profile?
- More before/after photos, ideally shot from the same spot (for a drag slider), and any snow jobs?
- Do you take seasonal snow contracts vs. per-storm? Any minimums or response time you're happy to promise?
- Any reviews from neighbors we can quote word for word?

## Ideas not built (yours to pick)
- **Runner-up world:** his crayon logo as the whole visual language (scribbled sky, crayon grass, the dachshund in the propeller cap as a recurring character). It's very much his, but it risks the "child's first digital art" look Ellie has rejected; it could work as accents (the dog walking along the footer lawn).
- The dachshund from the logo trotting across the bottom lawn, pushing leaves.
- A small reward when the hero lawn is fully raked (a neat pile appears, or rake stripes show).
- Season switch: after the first snow date, swap the hero to the snow scene and lead with snow shoveling.
- Before/after drag sliders once he sends same-spot pairs.
- Rake marks left behind in the grass where you dragged.
- A short "what's included in a fall cleanup" list if he gives one (gutters? haul-away? bagging?).

## Review notes
- Impeccable: critique, audit, harden, optimize, adapt, polish, layout, typeset, colorize, clarify, animate, delight, bolder, quieter and distill were all run (`live`, `onboard`, `shape`, `extract` don't apply). Their recommended fixes were applied, except the ones that break the house rules (listed as rejected in their reports).
- Finish reviewer (code-led, no comp): first verdict `fix` with 8 items. After two fix rounds all 8 were scored resolved. The final round found two small regressions (gaps in the leaf pile; the hint off the grid). I fixed both and checked them myself, with no third review round.
- Detector: the only finding still standing is `flat-type-hierarchy` (body sizes 15–20px). Ignored with reasons in `.impeccable/config.json`: `overused-font=roboto` (system stack is house style), `cream-palette` (oat is sampled from his flyer), `cramped-padding` (ruled rows; lawn flush to the footer).
- Desktop hero: the evaluate pass suggested putting a before/after on the right side. I filled it with the leaf pile instead. Say if you'd rather have the photo there.

## Not verified
- Real-device touch on iPhone/Android, inside Facebook's in-app browser (tested with simulated touch/pointer events in headless Chrome).
- The real SMS handoff on iOS and Android (`sms:+1…?&body=` format); desktop browsers usually do nothing on `sms:` links.
- Frame rate on older phones (phones draw ~250–300 leaves at ≤1.5× pixel ratio; one shared animation loop that pauses off screen).
- WebKit/Safari rendering (only Chrome was used headlessly).
