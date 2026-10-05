---
name: motion-graphics
description: Launch videos and Shorts written as code, shown as a photographic proof sheet of the engine's own frames.
colors:
  paper: "#e5e8e9"
  paper-hi: "#f3f5f6"
  paper-lo: "#d1d6d8"
  ink: "#151718"
  ink-2: "#464b4e"
  rebate: "#131313"
  rebate-2: "#222220"
  hole: "#34342f"
  emulsion: "#0a0a0a"
  rebate-note: "#b9b9b2"
  edge: "#f0a332"
  grease: "#c8271a"
  grease-deep: "#a91f13"
  comp-bg: "#101010"
  comp-card: "#1a1a19"
  comp-ink: "#eceae4"
  comp-dim: "#8d8a82"
  comp-red: "#e2311d"
typography:
  display:
    fontFamily: "Sofia Sans Extra Condensed, Arial Narrow, sans-serif"
    fontSize: "clamp(3.5rem, 6.6vw, 6rem)"
    fontWeight: 850
    lineHeight: 0.9
    letterSpacing: "-0.005em"
  headline:
    fontFamily: "Sofia Sans Extra Condensed, Arial Narrow, sans-serif"
    fontSize: "clamp(2.6rem, 5vw, 4.5rem)"
    fontWeight: 850
    lineHeight: 0.9
    letterSpacing: "-0.005em"
  title:
    fontFamily: "Sofia Sans Extra Condensed, Arial Narrow, sans-serif"
    fontSize: "clamp(2rem, 3.2vw, 2.8rem)"
    fontWeight: 850
    lineHeight: 0.95
  body:
    fontFamily: "Sofia Sans, system-ui, sans-serif"
    fontSize: "1.0625rem"
    fontWeight: 400
    lineHeight: 1.6
  label:
    fontFamily: "Sofia Sans Extra Condensed, Arial Narrow, sans-serif"
    fontSize: "12px"
    fontWeight: 650
    lineHeight: 1
    letterSpacing: "0.16em"
    fontFeature: "\"tnum\""
  mono:
    fontFamily: "JetBrains Mono, ui-monospace, monospace"
    fontSize: "14px"
    fontWeight: 400
    lineHeight: 1.7
  hand:
    fontFamily: "Covered By Your Grace, cursive"
    fontSize: "clamp(1.15rem, 1.5vw, 1.45rem)"
    fontWeight: 400
    lineHeight: 1.3
rounded:
  edge: "3px"
  pill: "4px"
  control: "6px"
  lens: "50%"
spacing:
  frame-gap: "clamp(3px, 0.5vw, 7px)"
  strip-gap: "clamp(10px, 1.3vw, 18px)"
  gutter: "clamp(20px, 4vw, 64px)"
  block: "clamp(40px, 6vh, 72px)"
  section: "clamp(72px, 11vh, 140px)"
components:
  install-command:
    backgroundColor: "{colors.rebate}"
    textColor: "{colors.paper-hi}"
    typography: "{typography.mono}"
    rounded: "{rounded.control}"
    padding: "15px 18px"
  copy-button:
    backgroundColor: "{colors.rebate}"
    textColor: "{colors.edge}"
    typography: "{typography.label}"
    padding: "0 18px"
  copy-button-hover:
    backgroundColor: "{colors.edge}"
    textColor: "{colors.rebate}"
  pill:
    backgroundColor: "{colors.rebate}"
    textColor: "{colors.edge}"
    typography: "{typography.label}"
    rounded: "{rounded.pill}"
    padding: "7px 12px"
  pill-hover:
    backgroundColor: "{colors.edge}"
    textColor: "{colors.rebate}"
  play-button:
    backgroundColor: "{colors.grease}"
    textColor: "{colors.paper-hi}"
    size: "64px"
  play-button-hover:
    backgroundColor: "{colors.grease-deep}"
  film-strip:
    backgroundColor: "{colors.rebate}"
    textColor: "{colors.edge}"
    padding: "0 clamp(6px, 0.8vw, 12px)"
  print:
    backgroundColor: "{colors.paper-hi}"
    padding: "clamp(8px, 1vw, 14px)"
  code-block:
    backgroundColor: "{colors.rebate}"
    textColor: "{colors.paper}"
    typography: "{typography.mono}"
    rounded: "{rounded.control}"
    padding: "22px 24px"
---

# Design System: motion-graphics

## Overview

**Creative North Star: "The Proof Sheet"**

Everything sits on a bench of photographic paper: a cool, faintly fibrous off-white ground on which black film strips, glossy prints, and an editor's marks are laid out. Real frames rendered by the engine are the imagery; the page never draws an illustration of a video when it can show the frame. Interface elements borrow their form from the darkroom: controls are cut from the same black stock as the film rebates, and the only small-label voice is the amber print found along a film edge.

Two hands touch the sheet. The typesetter sets huge, extra-condensed uppercase headlines and plain humanist reading text. The editor marks it up in red grease pencil: circles, crop corners, ticks, arrows, short handwritten notes, all drawn with a slightly waxy, wobbling stroke. Objects on the sheet are laid down by hand, so strips and prints sit a fraction of a degree off square and cast soft contact shadows on the paper.

Density is generous on the paper and tight inside the film. Wide sections breathe; the frames within a strip butt close together like a real contact print.

**Key Characteristics:**
- Cool photographic-paper ground with a fine noise texture, never flat white.
- Black film stock (rebates with sprocket holes) as the container for frames, steps, controls, and code.
- Amber edge print as the sole small-label voice; red grease pencil as the sole annotation voice.
- Extra-condensed uppercase display, humanist sans body, mono only for real code and commands.
- Slight hand-placed rotation and soft contact shadows on strips and prints.
- Motion as film advance, pencil draw-on, and loupe glide.

## Colors

A near-monochrome darkroom palette of cool paper and black film, lit by exactly two signal colors: amber edge print and red grease pencil.

### Primary
- **Grease Pencil Red** (grease): every hand annotation (circles, crop marks, ticks, arrows, handwritten notes), the emphasized phrase in a headline, the play control, the focus ring, and the text caret. Deepens to **Burnt Grease** (grease-deep) on hover of filled red controls.

### Secondary
- **Film-Edge Amber** (edge): small labels printed on black stock (frame numbers, t values, timecode, triangle markers), the text of controls cut from film stock, keywords in code, footer links, and the text selection fill. It appears only on black, never on paper.

### Neutral
- **Photographic Paper** (paper): the page ground, under a fine fractal-noise fibre.
- **Glossy Print White** (paper-hi): the border of prints, and light text on black stock.
- **Paper Shadow** (paper-lo): hairline section dividers, spec-table rules, scrollbar track.
- **Developer Black** (ink): headlines and primary text on paper; the heavy rule that opens a spec table.
- **Faded Ink** (ink-2): body copy, ledes, captions, and secondary text on paper.
- **Rebate Black** (rebate): film strips, the install command, code blocks, the transport, pills, the footer leader.
- **Rebate Seam** (rebate-2): the divider between the command and its copy button.
- **Sprocket** (hole): the sprocket-hole row on every strip and on the scrub track.
- **Emulsion** (emulsion): the empty frame behind images and live compositions before they load.
- **Rebate Note** (rebate-note): reading text on black stock (step descriptions).

### Composition palette
The demo compositions are the engine's output, framed by the page rather than placed on it. They run on their own dark set: **Stage Black** (comp-bg), **Stage Card** (comp-card), **Stage Ink** (comp-ink), **Stage Dim** (comp-dim, also the comment color in code blocks), and **Stage Red** (comp-red), with Film-Edge Amber shared with the page.

### Named Rules
**The Two Signals Rule.** Amber speaks for the film; red speaks for the editor. No third accent, and neither color is used as a decorative fill on paper.

**The Amber On Black Rule.** Amber text lives only on rebate black, where it reads; on paper it is never used for text.

## Typography

**Display Font:** Sofia Sans Extra Condensed (with Arial Narrow)
**Body Font:** Sofia Sans (with system-ui)
**Label/Mono Font:** JetBrains Mono for code and commands; Covered By Your Grace for grease-pencil handwriting

**Character:** The display face is the condensed grotesk of film-edge printing, set heavy and uppercase so headlines stack like a slate; the body face is a calm humanist companion from the same family. Handwriting is the editor, not decoration.

### Hierarchy
- **Display** (850, clamp(3.5rem, 6.6vw, 6rem), 0.9, uppercase, balanced wrap): the hero headline only.
- **Headline** (850, clamp(2.6rem, 5vw, 4.5rem), 0.9, uppercase, max 14ch): section headings.
- **Title** (850, clamp(2rem, 3.2vw, 2.8rem), 0.95, uppercase): format headings; step names on film stock run at 1.9rem.
- **Body** (400, 1.0625rem, 1.6): reading text; ledes run to 1.125–1.1875rem in Faded Ink, held to 34–40em.
- **Label** (650, 12px, 0.16em, uppercase, tabular figures): edge print on film stock and control labels.
- **Mono** (400, 14px, 1.7): code blocks; 500 weight in the install command; 600 tabular for timecode.
- **Hand** (400, about 1.15–1.6rem, 1.3, slightly rotated): grease-pencil notes and print captions.

### Named Rules
**The Real Code Rule.** Mono appears only for code and commands a reader could run. Never for labels or decoration.

**The One Edge Voice Rule.** Small uppercase labels exist only as edge print on film stock. Headings on paper stand alone with no label above them.

## Layout

A single centered column capped at 1360px with a fluid gutter. The hero is a 7:5 split with the contact sheet on the left and the copy on the right; the closing install block repeats the 7:5 split. Sections are separated by generous vertical padding and a hairline Paper Shadow rule. Content blocks under a section heading start one block step below the lede.

Film strips use a six-column frame grid with a tight frame gap; sprocket rows run above and below every strip. The six-step strip keeps a 1080px minimum and scrolls horizontally inside its own container rather than reflowing. Prints sit side by side in a 32:9 split, bottom-aligned, so the landscape and portrait prints share a baseline.

At 1100px and below, two-column splits stack and the hero copy moves above the sheet. At 760px and below, prints, code pairs, and format columns stack; QA strips drop to three columns; nav collapses to the GitHub link alone.

## Elevation & Depth

Depth is physical: objects lying on a paper bench. Strips, prints, code blocks, and the install command cast soft, low contact shadows tinted black; nothing glows and nothing floats high. The loupe is the one raised object, carrying a black rim and the deepest drop. A slight rotation on strips and prints (−0.5° to 1.2°) does as much depth work as the shadows do.

### Shadow Vocabulary
- **Strip contact** (`box-shadow: 0 2px 2px rgba(0,0,0,.18), 0 14px 26px -16px rgba(0,0,0,.55)`): film strips on paper.
- **Print contact** (`box-shadow: 0 1px 1px rgba(0,0,0,.12), 0 24px 40px -22px rgba(0,0,0,.5)`): glossy prints.
- **Stock low** (`box-shadow: 0 10px 24px -14px rgba(0,0,0,.6)`): install command and code blocks.
- **Loupe** (`box-shadow: 0 0 0 3px var(--rebate), 0 22px 40px -12px rgba(0,0,0,.55)`): the magnifier lens only.

### Named Rules
**The Bench Rule.** Every shadow is a soft contact shadow from an object resting on paper. No hard offset shadows, no colored glows.

## Shapes

Film stock is cut square: strips, steps, and frames have no radius. Controls cut from black stock get small corners (pill 4px, install command, code blocks, and transport 6px). Prints are square-cornered with a white border. The loupe is the one circle. Sprocket holes are drawn as repeating gradients, not images. Grease-pencil strokes are round-capped SVG paths roughened by a wax displacement filter.

## Components

### Buttons
Controls are pieces of film stock: black with amber label print, flipping to an amber fill with black text on hover.
- **Copy button:** attached to the right of the install command behind a Rebate Seam divider; label type; hover inverts to amber fill; after copying, the label reads "Copied" in Glossy Print White.
- **Pill:** small play/pause toggle with a 12px inline SVG; same inversion on hover.
- **Play button:** the one filled red control, a 64px square (52px on small screens) at the head of the transport; deepens on hover.
- **Focus:** a 2px Grease Pencil Red outline offset 3px; on frames inside a strip the outline turns amber.

### Install command
A black strip holding the command in mono with the executable highlighted amber, and the copy button flush right. It appears in the hero and again at the close, always as a working control.

### Film strip (signature)
Black rebate with sprocket rows top and bottom, an amber edge-print row of frame numbers and triangle markers above the frames, and t values or stock codes below. Frames are 16:9 (or 9:16 for Shorts) real engine renders. Strips enter by advancing sideways one frame.

### Print
A glossy white-bordered photograph of a live composition or still, slightly rotated, with grease-pencil crop corners drawn on and a caption row: handwritten title on the left, mono specification on the right.

### Loupe (signature)
A circular lens with a black rim that glides after the pointer across the contact sheet and plays the live composition from the frame beneath it, with an amber t readout on a small black tab below. When the pointer leaves, it parks on the circled keeper frame.

### Transport
A black bar: red play button, a scrub track with sprocket rows and amber second ticks, an amber playhead with a soft halo, and mono timecode in amber.

### Spec table
A two-column definition list opened by a 2px Developer Black rule, with hairline Paper Shadow rules between rows and semibold terms.

### Navigation
A plain header: the wordmark in display type beside a small film-frame mark, and three text links at 600 weight. Links take Grease Pencil Red on hover.

## Do's and Don'ts

### Do:
- **Do** show real engine frames and live compositions as the imagery; every frame shown should be one the engine rendered.
- **Do** put amber labels only on rebate black, set in label type with tabular figures.
- **Do** mark up content in grease pencil (circles, crop corners, ticks, arrows, short handwritten notes), drawing on with stroke-dashoffset when it enters view.
- **Do** lay strips and prints a fraction of a degree off square with soft contact shadows.
- **Do** use the shared ease-out curve (cubic-bezier(.16, 1, .3, 1)) for film advance, draw-on, and control transitions, and drop the animations under prefers-reduced-motion.
- **Do** keep content visible by default; motion only enhances it.

### Don't:
- **Don't** introduce a third accent color or use amber or red as a fill on paper.
- **Don't** set small uppercase labels or eyebrows above headings on paper; edge print belongs to film stock.
- **Don't** use mono for anything but code and commands.
- **Don't** use hard offset shadows or glows; depth is soft contact shadow and rotation.
- **Don't** round film stock; only controls get small corners and only the loupe is circular.
- **Don't** use icon fonts or glyph characters as icons; icons are small inline SVGs in currentColor.
