---
version: alpha
name: "Perfumery template by 8B"
description: "A dark, quiet one-page design for an independent perfumery that sells by appointment and by post: near-black ground, warm cream type, amber thread lines and arched photo windows. Free HTML template by 8B, MIT."
colors:
  primary: "#141213"
  secondary: "#f1eade"
  tertiary: "#b48a5a"
  neutral: "#ffffff"
  surface: "#141213"
  on-surface: "#f1eade"
  surface-light: "#f1eade"
  on-surface-light: "#141213"
  brown-deep: "#573726"
  brown-mid: "#8c5f43"
  caption-light: "#675a50"
  caption-dark: "#a99d91"
  accent-amber: "#b48a5a"
typography:
  headline-display:
    fontFamily: Kalnia
    fontSize: 112px
    fontWeight: 300
    lineHeight: 0.88
    letterSpacing: -0.025em
  headline-md:
    fontFamily: Kalnia
    fontSize: 30px
    fontWeight: 400
    lineHeight: 1.08
    letterSpacing: -0.01em
  tagline:
    fontFamily: Kalnia
    fontSize: 24px
    fontWeight: 400
    lineHeight: 1.04
    letterSpacing: -0.01em
  body-md:
    fontFamily: Host Grotesk
    fontSize: 17px
    fontWeight: 400
    lineHeight: 1.5
  label-md:
    fontFamily: Host Grotesk
    fontSize: 13px
    fontWeight: 500
    lineHeight: 1.3
    letterSpacing: 0.01em
  lead-caps:
    fontFamily: Host Grotesk
    fontSize: 21px
    fontWeight: 400
    lineHeight: 1.2
  button:
    fontFamily: Host Grotesk
    fontSize: 12px
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: 0.04em
  badge:
    fontFamily: Host Grotesk
    fontSize: 11px
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: 0.05em
  field-input:
    fontFamily: Kalnia
    fontSize: 34px
    fontWeight: 300
    lineHeight: 1.2
    letterSpacing: -0.01em
rounded:
  sm: 4px
  md: 8px
  full: 999px
  card: 22px
spacing:
  gutter: 56px
  button-min-height: 54px
  nav-pill-height: 34px
components:
  button-primary:
    backgroundColor: "{colors.neutral}"
    textColor: "{colors.primary}"
    typography: "{typography.button}"
    rounded: "{rounded.sm}"
    padding: 10px 11px 12px 12px
    height: 54px
  button-secondary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.secondary}"
    typography: "{typography.button}"
    rounded: "{rounded.sm}"
    padding: 10px 11px 12px 12px
    height: 54px
  nav-pill:
    backgroundColor: "#33302f"
    textColor: "{colors.secondary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.sm}"
    padding: 6px 16px
    height: 34px
  card-extrait:
    backgroundColor: "{colors.secondary}"
    textColor: "{colors.primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.md}"
    padding: 12px 16px 14px
  badge-status:
    textColor: "{colors.primary}"
    typography: "{typography.badge}"
    rounded: "{rounded.full}"
    padding: 3px 11px
  input-field:
    textColor: "{colors.primary}"
    typography: "{typography.field-input}"
    rounded: "0"
    padding: 4px 0
  tasting-strip:
    backgroundColor: "{colors.secondary}"
    textColor: "{colors.primary}"
    typography: "{typography.headline-md}"
    rounded: 3px
  footer-card:
    backgroundColor: "{colors.neutral}"
    textColor: "{colors.primary}"
    rounded: "{rounded.card}"
    padding: 44px
---

## Overview

The Resin Cabinet is a one-page design for an independent perfumery that sells by appointment and by post. Its one idea is that scent comes before the name: strips are shown unnamed, so the page withholds as much as it shows. A near-black ground carries cream type, and amber thread lines wander behind the light sections like a scent trail. It is made for a small maker with a few signature products who wants a quiet, editorial page, not a shop front. The feeling is a room with no window: low light, careful type, no noise.

## Colors

Eight colours come from `:root`, plus one derived tint. Dark sections and light sections alternate down the scroll.

- **Near-black `#141213` (primary):** page ground, the solid nav bar, the opening second screen, origins, noses and the footer. On the cream and white sections it is the text colour.
- **Cream `#f1eade` (secondary):** type on dark sections, ground of shelf, accord, resting, questions and visit, the four tasting strips and the numbered vial discs.
- **Amber `#b48a5a` (tertiary):** thread lines on the cream sections and in the footer card, and the ring around the count of scents on the shelf. Use it only as a line.
- **White `#ffffff` (neutral):** cabinet section ground, the footer card, the primary button and the menu button, and the thread line on the visit section.
- **Deep brown `#573726`:** the sample set section ground, the start of the first-screen gradient and the portrait arch backing.
- **Mid brown `#8c5f43`:** the lower end of the first-screen gradient.
- **Caption on light `#675a50`:** small print, batch numbers, note labels, answers and placeholders on light sections.
- **Caption on dark `#a99d91`:** secondary text on dark sections, such as the origin places and portrait bios.
- **Nav pill `#33302f`:** the resting fill of the header pills is cream at 14 percent opacity; it reads as `#33302f` over the solid near-black bar and warmer over the opening gradient.

## Typography

Two families, both loaded in two weights. **Kalnia** is a serif used light (300) for the large display lines and section headings, and regular (400) for the smaller serif lines: extrait names, tag lines, form fields and the vertical words on the strips. Display sizes use `clamp()`: the base heading runs from 48px to 112px, and individual sections go larger, up to 184px on the opening heading. Tracking is slightly negative and line height is 0.88, so lines sit tight. **Host Grotesk** is the sans for body text (17px on desktop, 15px on small screens), 13px labels and captions, and 12px uppercase button labels at weight 500 with wide tracking. Do not add a third face.

## Layout

The page is full width with a side gutter of 4vw, from 16px up to 56px. Sections breathe with about 16vh of vertical padding. Headings step to the right line by line, so each one reads like a staircase; the same stepping appears in tag lines and the footer links. Content sits on a 12-column grid in the shelf and footer, a 5 to 7 split in questions and the sample set, a 7 to 4 split in visit, and a six-tile grid in origins. Below 860px the two-column sections become one column and the header pills hide behind the menu button; below 768px the cabinet shows two cards across with the three note rows run together, separated by slashes.

## Elevation & Depth

Depth comes from layers, not from shadows. The opening has an arch, two tilted photo cards and a rising ink dome stacked over a brown gradient. One shadow token exists, a long soft drop (`0 24px 60px -24px`, near-black at 70 percent), used under the floating opening cards, the shelf photo and the cabinet cards once they are pinned. Section edges change from dark to cream with no divider.

## Shapes

Corners are quiet: 4px on buttons, header pills and strips (3px), 8px on photos and extrait cards, and 22px on the white footer card. Portraits and the opening photo sit in arches, a top corner radius of 999px with square feet. Badges and the shelf number are pills and circles. Form fields have no box, only a hairline under them. Amber and white thread lines are 1 to 1.2px hairlines drawn as SVG paths.

## Components

- **button-primary:** white tile with an uppercase label at the top left and a small dot at the bottom right; on hover the dot grows into a near-black fill and the label turns cream.
- **button-secondary:** the same tile in near-black, used on cream sections, filling with cream on hover.
- **nav-pill:** a translucent cream pill in the header; it fills solid cream on hover. The menu opens a full-screen near-black layer with five large staggered links.
- **card-extrait:** cream card with a photo, number, name, three note rows and a 50 ml price under a hairline.
- **badge-status:** outlined uppercase pill for batch status.
- **input-field:** a large light serif input over a hairline, with a stacked two-line label at the left.
- **tasting-strip:** a cream paper strip with a vertical serif word and a letter tag.
- **footer-card:** a white rounded card on the dark ground with the amber thread and the giant footer links.

## Motion

The page loads GSAP, ScrollTrigger, SplitText and Lenis from jsDelivr; Lenis gives smooth scrolling. The one motion idea is parting and dealing: things start together and move apart as you scroll.

- **Opening:** on load the heading lines rise, the arch and cards slide in, the cards float and the arch photo pans slowly. On scroll the first screen stays pinned for about one screen while the heading parts left and right, the cards fly up, an ink dome rises over it and four strips slide in from the centre.
- **Origins:** pinned for about 1.4 screens; the middle photo fills the stage, shrinks into its slot and the other five tiles fly in, turning as they land.
- **Cabinet:** pinned for about 2.3 screens; two title words part to the edges while four cards are dealt out of a stack.
- **Accord:** a resin photo splits down the middle and its two halves slide apart to frame a bottle photo that settles from a zoom.
- **Noses:** the huge word slides in from the right, and three portraits open from a narrow arch to full width.
- **Sample set:** six round openings widen until the whole photo shows.
- **Headings and lines:** headings rise from a line mask, tag lines settle in from the left, and thread lines draw with scroll.

With reduced motion the entrance and scroll animations and smooth scrolling are off and the page reads as a plain stack of sections. Hover fills and the nav's hide on scroll keep running.

## Do's and Don'ts

- Do keep the near-black and cream alternation, with white and deep brown as the only other grounds; add no new ground colour.
- Do use amber only as a thread line or a thin ring.
- Do step display lines to the right and keep the tight 0.88 line height.
- Do keep corners at 3 to 8px, and arches for portraits.
- Do show things unnamed first: strips and cards carry numbers before names.
- Don't add drop shadows to flat sections, gradients on buttons or a second display face.
- Don't use icons or emoji for notes or ingredients; the type carries them.
- Don't add motion that does not part, deal or draw; keep it slow and scrubbed to scroll.
