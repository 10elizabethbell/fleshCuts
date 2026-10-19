---
name: FleshCuts LLC
description: A neighbor's yard you can rake yourself; fall cleanups and snow shoveling in Brick, NJ.
colors:
  forest: "#1c3a29"
  forest-deep: "#142c1e"
  forest-hi: "#26503a"
  amber: "#e49a3c"
  amber-hi: "#f0ab52"
  amber-deep: "#cf8326"
  rust: "#a8401a"
  oat: "#efe5d3"
  oat-line: "rgba(26,43,33,.16)"
  snow: "#eef4f7"
  paper: "#f8f2e7"
  ink: "#1a2b21"
  ink-soft: "#46564c"
  cream: "#f6efe2"
  cream-soft: "#d9d2c2"
  error: "#9b2c12"
typography:
  display:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", Roboto, \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "clamp(2.6rem, 11.4vw, 5.6rem)"
    fontWeight: 900
    lineHeight: 0.93
    letterSpacing: "-0.01em"
  headline:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", Roboto, \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "clamp(2rem, 8.6vw, 3.6rem)"
    fontWeight: 900
    lineHeight: 0.98
    letterSpacing: "-0.01em"
  title:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", Roboto, \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "clamp(19px, 5.2vw, 24px)"
    fontWeight: 800
    lineHeight: 1.2
    letterSpacing: "-0.005em"
  body:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", Roboto, \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "17px"
    fontWeight: 400
    lineHeight: 1.5
  label:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", Roboto, \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "17px"
    fontWeight: 800
    lineHeight: 1.2
rounded:
  pill: "999px"
  photo: "14px"
  control: "12px"
  card: "20px"
  circle: "50%"
spacing:
  pad-phone: "16px"
  pad-tablet: "32px"
  pad-desktop: "48px"
  band: "64px"
  band-desktop: "96px"
components:
  button-primary:
    backgroundColor: "{colors.amber}"
    textColor: "{colors.forest}"
    typography: "{typography.label}"
    rounded: "{rounded.pill}"
    padding: "0 22px"
    height: "56px"
  button-primary-hover:
    backgroundColor: "{colors.amber-hi}"
    textColor: "{colors.forest}"
  button-outline:
    backgroundColor: "transparent"
    textColor: "{colors.cream}"
    typography: "{typography.label}"
    rounded: "{rounded.pill}"
    padding: "0 22px"
    height: "56px"
  service-row:
    backgroundColor: "transparent"
    textColor: "{colors.ink}"
    typography: "{typography.title}"
    padding: "10px 0"
    height: "68px"
  service-row-arrow:
    backgroundColor: "transparent"
    textColor: "{colors.ink}"
    rounded: "{rounded.circle}"
    size: "44px"
  service-row-arrow-hover:
    backgroundColor: "{colors.amber}"
    textColor: "{colors.forest}"
  facebook-link:
    backgroundColor: "{colors.forest}"
    textColor: "{colors.cream}"
    rounded: "{rounded.pill}"
    padding: "0 24px"
    height: "64px"
  facebook-link-hover:
    backgroundColor: "{colors.forest-hi}"
  input-text:
    backgroundColor: "#ffffff"
    textColor: "{colors.ink}"
    typography: "{typography.body}"
    rounded: "{rounded.control}"
    padding: "13px 14px"
    height: "52px"
  choice-chip:
    backgroundColor: "#ffffff"
    textColor: "{colors.ink}"
    rounded: "{rounded.control}"
    padding: "0 16px"
    height: "48px"
  quote-card:
    backgroundColor: "{colors.paper}"
    rounded: "{rounded.card}"
    padding: "22px 18px"
---

# Design System: FleshCuts LLC

## Overview

**Creative North Star: "The Yard Is the Page"**

The page is Brandon's own October lawn, not a picture of one. The flyer's deep forest green and oat beige carry the brand; canvases of mown turf covered in maple, oak and beech leaves sit at the bottom of the hero, under every before/after pair and above the footer, and the visitor rakes them with a finger or cursor. Winter comes in as a pale-blue sky strip where snow falls, banks up and can be shovelled. Everything else stays plain so the yard can be the one living thing on the page.

The type is loud and the furniture is quiet. Headlines are heavy, uppercase and tight in the system face. Content sits on flat color bands (forest, oat, snow) separated by organic edges: a cut turf edge with a strip of soil, a wavy oat edge over the snow, a drift-shaped mask into the estimate band. Controls are few and large: one amber pill to text Brandon, one outlined pill for the second action, ruled rows of services that text him with a single tap.

Density is phone-first and generous: 56px buttons, 68px rows, 17px body, one column until 1024px, where bands split into a sticky heading column beside the content.

**Key Characteristics:**
- Flat color bands from the owner's flyer (forest, oat, pale blue), joined by organic, hand-cut edges rather than straight rules.
- Heavy uppercase system type (900 weight, line-height under 1) for every heading; plain sentence-case body.
- One amber action color, shown at rest only on the primary pill; everywhere else amber appears on hover.
- A rust outline reserved for form controls.
- A living yard (LeafLawn and SnowBank canvases) that plays by itself until touched and never moves under reduced motion.

## Colors

The flyer's forest and oat, lifted into October with leaf amber, plus a pale-blue snow band for winter.

### Primary
- **Flyer Forest** (forest): the hero and the close section, the numbered step discs, the Facebook link pill, and the text color on amber. It is the owner's own ad green and the ground every light element sits on.
- **Night Forest** (forest-deep): footer only, so the page ends a step darker than the close.
- **Lit Forest** (forest-hi): hover fill of the forest pill.

### Secondary
- **Leaf Amber** (amber): the primary button fill, the arrow-circle fill on row hover, the global focus ring, icons on forest (phone, Facebook, step numbers), selection highlight.
- **Sunlit Amber** (amber-hi): primary button hover.
- **Turned Amber** (amber-deep): border of a checked form chip, over a pale amber tint (#fbe8cf).

### Tertiary
- **Rust** (rust): the form's hover and focus outline (2px border plus a 3px rust halo at 18-22% alpha), and the text caret. It exists so the form outline stands out from the amber button it surrounds.

### Neutral
- **Oat** (oat): page ground and the fall and estimate bands; the flyer's beige.
- **Oat Rule** (oat-line): the 1px rules between service rows and above the form fallback.
- **Snow** (snow): the snow-shoveling band and the bank's base color; the flyer's pale blue, lifted.
- **Paper** (paper): the quote form card.
- **Ink** (ink) and **Soft Ink** (ink-soft): text on oat, snow and paper; soft ink for band ledes, photo labels, help text and "(optional)".
- **Cream** (cream) and **Soft Cream** (cream-soft): text on forest; soft cream for the outline button's border, the rake hint, the service-area line and the footer.
- **Error Brick** (error): form error messages only.

Leaf colors live in the engine, not on :root: rust #c4521f, orange #d9822b, gold #e2ad37, maroon #8f2f1d, tan #9a6430, copper #b8681f, ochre #c9a13a. Grass blades use six greens from #27502a to #5a8a45 over a #2b5229 to #3b6c35 turf gradient.

### Named Rules
**The Amber on Touch Rule.** Amber at rest is for the primary button only. Arrows, links and the phone number turn amber when hovered or focused, never by default.

**The Rust Is the Form Rule.** Rust outlines only form controls: text boxes, choice chips, the form's submit and copy buttons. Nothing outside the form uses rust.

**The Flyer Ground Rule.** Large surfaces come from the owner's flyer: forest, oat, pale blue. Don't introduce a new band color.

## Typography

**Display Font:** System stack (-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial)
**Body Font:** The same system stack

**Character:** One family at two extremes: 900-weight uppercase headings set almost solid, against 17px sentence-case body that reads like a text from a neighbor. The system face is Ellie's house type for these sites (ellie-taste.md section 2).

### Hierarchy
- **Display** (900, clamp 2.6rem to 5.6rem, line-height 0.93, uppercase, max 13ch): the hero headline only, in white with a soft forest glow (0 2px 24px at 60%) so it holds over the leaves.
- **Headline** (900, clamp 2rem to 3.6rem, 0.98, uppercase): band headings ("Fall cleanups", "Snow shoveling", "Free estimates") and the close. Sub-headings step down within the same voice: "Cleanup results" at clamp 1.7rem to 2.8rem, the about heading at clamp 1.9rem to 3.2rem.
- **Title** (800, clamp 19px to 24px): service row names.
- **Body** (400, 17px, 1.5): running text. Ledes and step text at 18px, the hero promise at clamp 17px to 20px with max 32ch, about copy at max 46ch.
- **Label** (800, 16-18px): buttons, form labels and legends, Before/After labels, the header phone number (tabular figures).
- **Small** (15-16px): help text, errors, rake hint, footer.

### Named Rules
**The Heavy Caps Rule.** Every h1-h3 is 900 weight, uppercase, -0.01em, line-height under 1, balanced. Body copy is never uppercase.

**The One Family Rule.** No second typeface. Hierarchy comes from weight, case and size only.

## Layout

A centered column (max 1160px) with side padding of 16px on phones, 32px from 700px and 48px from 1024px. Bands are 64px top and bottom, 96px from 1024px.

- **Phone (default):** one column. Hero fills 100svh, with the lawn taking the bottom clamp(170px, 31svh, 260px) (110px in short landscape). Hero buttons stack full width.
- **700px:** hero buttons sit in a row (min 250px each); before/after pairs go side by side; lawn strips widen to the full viewport; the snow seam grows from 150px to 190px.
- **1024px:** fall and snow bands split 5:7 with the heading column sticky at 32px; the estimate band splits 5:6 with the steps sticky beside the form; the about block puts the logo beside the text; the close CTA puts its button to the right of the heading.

The first screen is fixed: logo and name top left, the phone number top right as a tel: link, the headline, one promise line, two buttons, then the lawn. There is no sticky bottom bar at any width.

### Named Rules
**The Clear Copy Rule.** Nothing in the yard crosses the words. Leaves stay low over the hero copy and fly high only to the right of it, below the header.

## Elevation & Depth

Flat bands with soft, warm, downward shadows on the few objects that sit on them. No hard offset shadows, no glows on controls.

### Shadow Vocabulary
- **Photo rest** (`box-shadow: 0 10px 22px -14px rgba(74,48,20,.35)`): before/after photos.
- **Card rest** (`box-shadow: 0 18px 40px -24px rgba(74,48,20,.5)`): the quote form card.
- **Logo lift** (`box-shadow: 0 20px 44px -18px rgba(0,0,0,.55)`): the round logo on forest in the about block; the header logo has a small 0 2px 8px at 25%.
- **Form halo** (`box-shadow: 0 0 0 3px rgba(168,64,26,.18)`): state, not elevation; see Inputs.

Depth in the yard comes from painting, not CSS: leaf drop shadows, pile shadows, mown stripes, the shaded bank crest.

## Shapes

Round where touched, soft where shown, organic where nature meets the layout.

- **Pills** (999px): every button and the Facebook link.
- **Circles** (50%): arrow circles, step numbers, logos.
- **Photos** (14px), **controls** (12px), **form card** (20px), **chip checkbox** (5px).
- **Edges between bands are never ruled straight:** the turf ends in a wavy cut edge with a soil strip (#4a321e) before the next band's color; the oat band ends in a wavy edge over the snow; the estimate band starts under a drift-shaped mask. Only list rows use straight 1px rules.

## Components

### Buttons
Big, round and few.
- **Shape:** full pill (999px), min-height 56px, 22px side padding, 2px border, 800 weight at 17px, icon gap 0.55em.
- **Primary (amber fill):** amber with forest text and the text-bubble icon. It is the main action ("Text me for a free estimate", "Text this to Brandon"). Hover goes to sunlit amber; press scales to 0.98.
- **Secondary (outline):** transparent with a soft cream border and cream text, used on forest ("Book snow shoveling"). Hover turns the border amber and the text white.
- **At most two under the hero headline**, primary first. Neither is a call button; the phone number is the call.

### Service Rows
Ruled list rows that open a pre-filled text.
- **Structure:** 800-weight title left, a 44px arrow circle right, 68px min height, a 1px oat rule above the list and below each row.
- **Rest:** the arrow circle is neutral, with a 2px ink border at 22% alpha.
- **Hover / focus:** only the arrow changes: it fills amber with a forest arrow. The row gets no outline, background or shadow. The keyboard focus ring (3px amber, 3px offset) goes on the arrow circle, not the row.

### Inputs / Fields
- **Text boxes:** white, 2px ink border at 20% alpha, 12px radius, 52px min height (textarea 96px, no resize), 17px text. Labels are 800 weight above the field; optional fields say "(optional)" in soft ink.
- **Choice chips:** real checkboxes behind 48px rounded tiles with a drawn 18px box; checked = pale amber tint, turned-amber border, forest box with an amber tick.
- **Hover and focus:** every control in the form, including the submit and copy buttons, gets a rust border and a 3px rust halo. Native outline is suppressed in favor of this.
- **Errors:** error brick, 15px, 700 weight, under the field; empty errors take no space.
- **Hand-off:** submit composes an SMS; a fallback block shows the message to copy if the text app doesn't open.

### Navigation
No menu. The header holds the brand (42px round logo on white plus the 900-weight name) and the phone number with an amber icon, which turns amber on hover. The footer repeats the number and the Facebook link with amber icons on night forest.

### Before/After Pair on a Lawn
Each pair is two photos at their own 712:381 shape with plain "Before" / "After" labels and no captions, side by side from 700px. A 96px (120px desktop) leaf-covered lawn strip overlaps the bottom of the pair by 34px (40px), runs edge to edge, and ends in a soil edge into oat. It does not autoplay; it reacts to the pointer and lets vertical scrolling through (pan-y). Directly under the pairs is the Facebook link: a 64px forest pill with an amber Facebook mark, "Click to see more of my work.", with a lit-forest hover.

### Numbered Steps
Three plain steps, each with a 44px forest disc holding an amber 900-weight numeral and 18px text. Not interactive and not styled like buttons.

### The Living Yard (signature)
Two canvas scenes, LeafLawn and SnowBank, driven by one shared requestAnimationFrame loop.

**LeafLawn** paints mown turf (diagonal stripes, thousands of blades, swaying tips that bend away from the pointer and spring back) and scatters leaf sprites in three shapes (maple, oak, beech), seven colors, front and back faces with veins, each with a soft shadow. Leaves are pushed, lifted and flipped by the pointer, fall under gravity, flutter, and settle face up or face down. A leaf pushed off the lawn regrows after REGROW seconds, fading back in. A breeze nudges a few resting leaves so the lawn never sits still. Instances:
- **Hero:** autoplay; after IDLE seconds without a touch an unseen gust rakes a looping path across the lawn. The first touch hides the "Drag across the lawn" hint (it also fades by itself after 9s). The hit area is the lawn strip with touch-action none, so a drag works in every direction on a phone.
- **Desktop hero (from 700px, with 420px+ free to the right of the copy):** a raked leaf pile on the open right side, built from 420 leaves on fixed slots shaped like a mound. Only a real pointer can knock leaves out of the pile; regrowing leaves can drop back into empty slots, and leaves keep drifting down through the clear zone.
- **Height cap:** a leaf may rise only a little above its spot on the lawn, except to the right of the copy (measured from the headline, promise and buttons, plus 40px), where it can fly up to 96px under the top. This keeps leaves out of the words.
- **Under each photo pair** (density 0.85, no autoplay) and **above the footer** (150px, 190px desktop; density 0.8, autoplay, edged into night forest).

**SnowBank** fills the 150px (190px desktop) seam between the fall and snow bands: falling flakes that drift and land into a column heightmap (4px columns, max 52% of the height), so the bank grows; a drag shovels a dip under the pointer and throws lumpy, shaded snow clumps with powder puffs that land back on the bank. The bank smooths itself each frame, and after IDLE seconds an unseen shovel clears a pass every 9s. The crest is shaded white to snow with a faint blue shadow above it; the oat band above ends in a wavy edge.

**Loop and motion floor.** One rAF loop steps every visible scene and stops when none is visible; each canvas has an IntersectionObserver (80px margin) that pauses it off screen and wakes the loop. Device pixel ratio is capped at DPR_CAP. Pointer state is shared and read in client coordinates every frame. With prefers-reduced-motion, every scene draws one still frame (redrawn on resize), the gust and shovel never run, and smooth scrolling is off.

**Tunables** (named constants at the top of the engine script, tuned by hand): DPR_CAP 1.5; LEAF_DENSITY 230 (lawn px² per leaf); LEAF_MAX 650; LEAF_LEN 17-30px on phones, LEAF_LEN_DESK 22-36px; PUSH_R 46 / PUSH_R_DESK 64; REGROW 1.4-6s; IDLE 6s; GRAVITY 380, FALL_MAX 78; SNOW_FLAKES 70 / SNOW_FLAKES_DESK 170; LEAF_COLORS; GRASS.

## Do's and Don'ts

### Do:
- **Do** put the phone number only in the top-right corner of the header on the first screen, as a tel: link with a phone icon. The footer may repeat it.
- **Do** keep at most two buttons under the hero headline: amber-fill primary, cream-outline secondary.
- **Do** put the Facebook link directly under the before/after pairs as a 64px forest pill, and again in the footer.
- **Do** keep service items to one to three words in ruled rows where only the arrow circle changes on hover (amber fill, focus ring on the arrow).
- **Do** outline every form control in rust (2px border plus 3px halo) on hover and focus.
- **Do** keep photos at their own 712:381 shape with 14px corners, plain Before/After labels and a lawn strip tucked under each pair.
- **Do** tune the yard through the named constants at the top of the script, not inline numbers.
- **Do** keep every animation behind the shared loop, paused off screen and drawn as a still frame under reduced motion.

### Don't:
- **Don't** add a sticky bar at the bottom of the screen, a Call button under the hero title, or a second copy of the phone number on the first screen.
- **Don't** add email links, buttons or a "send by email" option; contact is call or text.
- **Don't** outline, tint or shadow a service row on hover.
- **Don't** use rust outside the form or amber at rest outside the primary button.
- **Don't** let leaves, flakes or clumps cross the hero copy; respect the height cap and the clear zone.
- **Don't** add captions under the photos or an intro sentence above them.
- **Don't** draw ruler-straight edges between bands; the yard's edges are cut turf, soil and drift.
- **Don't** add a second typeface or set body copy in uppercase.
