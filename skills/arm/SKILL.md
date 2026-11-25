---
metadata:
  internal: true
name: arm
version: 0.1.0
description: "Official U.S. Department of Energy Atmospheric Radiation Measurement (ARM) User Facility presentation template. Features the official ARM binary-cloud sky banner, ARM horizon logo, 9-National-Laboratory partner bar, and DOE Office of Science footer chrome across light-blue, green, purple, dark-blue, and gray themes. Use whenever the user asks for an ARM presentation, ARM template, DOE Office of Science atmospheric or climate deck, field campaign briefing, or ASR/ARM science talk."
inspiration: "Official U.S. DOE ARM User Facility PowerPoint template (arm-pptx-template.pptx), DOE Office of Science BER briefings, ARM/ASR Joint Principal Investigators Meeting presentations, National Laboratory technical reviews"
typography_kit: "Plus Jakarta Sans / Calibri / Arial 700 for banner headlines and section titles, Calibri / Arial 400/600 for structured body copy, IBM Plex Mono 500 for sensor telemetry, units, and site codes"
color_kit: "White stage (#FFFFFF), ice-slate card tint (#F4F7FA), charcoal ink (#2B2B2B), ARM Navy Blue (#194173), Primary Blue (#0070C1), Light Sky Blue (#80B8E0), ARM Green (#00BD70), ARM Purple (#99559F), Gold (#F7C446), and footer slate (#707276 / #828282)"
image_style: "Engine-rendered scientific charts, vertical profiles, instrument tables, and labeled placeholder frames for observatory or field-campaign photography; bleed slides use the official ARM binary-cloud sky backgrounds"
forbidden: "startup gradients, neon dark-mode cyber aesthetics, rounded-pill cards over 4px, card-edge accent borders, uppercase tracked-out labels, font sizes below 14px, em-dashes in rendered copy, fabricated observational datasets"
---

# ARM User Facility — Official Presentation Style Guide

This skill implements the official U.S. Department of Energy (DOE) Atmospheric Radiation Measurement (ARM) User Facility presentation template (`arm-pptx-template.pptx`). Every slide reproduces the authentic ARM master geometry, color palette, header cloud banner, 9-National-Laboratory partner strip, and DOE Office of Science footer.

## Voice

Clear, scientific, evidence-driven, and precise. Headlines state the scientific finding, operational milestone, or campaign objective directly. Measurements carry explicit physical units (W/m², GHz, km, TB/day, UTC). Acronyms common to the community (IOP,AAF, SGP, NSA, ENA, VAP, ASR, BER) are paired with concise context when introduced.

## Structure

1. **Cover (`cover`)** — Official ARM Title Slide with full-bleed binary-cloud sky background (`preset=sky|green|purple|navy|gray`), top-right ARM horizon logo, presentation title, presenter name(s), organization, event/location, the `#194173` 9-National-Laboratory partner bar, and the white DOE Office of Science footer strip.
2. **Section Dividers (`section-divider`, `section-split`)** — Either the full-bleed binary-cloud section divider (`slideLayout38`) or the diagonal split section divider with an image/exhibit frame (`slideLayout31`).
3. **Core Content & Comparisons (`standard`, `comparison`, `picture-caption`)** — Direct counterparts to the official ARM Master content layouts (`Standard Slide`, `Title + 2-Column Comparison with Titles`, and `Title + Picture with Caption`), upgraded with structured visual rhythm so slides never underfill.
4. **Scientific & Operational Exhibits (`metrics`, `time-series`, `bar-analysis`, `instrument-table`, `architecture`, `roadmap`)** — Quantitative exhibits for campaign telemetry, radiative flux closure, radar/lidar specifications, data-pipeline tiers, and multi-year schedules.
5. **Closing (`closing`)** — Full-bleed ARM summary, acknowledgments, and contact slide with the 9-Lab partner bar and DOE Office of Science footer.

## Visual system

- **Page & Stage**: 1920×1080 canvas. Content slides carry the official `176px` top binary-cloud header banner (`#194173` / `#0070C1` / `#80B8E0`) with the slide title set in bold white (`38px–42px`) on the left and the white ARM wordmark + horizon arc on the right (`x = 1620..1860px`).
- **Official ARM Palette**:
  - Charcoal Ink (`#2B2B2B`) on a crisp White stage (`#FFFFFF`) with soft ice-slate (`#F4F7FA`) exhibit cards and `#D5DCE4` hairline rules.
  - Primary Blue (`#0070C1`) and ARM Navy (`#194173`) carry primary structural headers, comparison banners, and numbered markers.
  - ARM Green (`#00BD70`), Light Sky Blue (`#80B8E0`), ARM Purple (`#99559F`), and Gold (`#F7C446`) encode multi-series data, theme variants, and status chips.
- **Footer Chrome**: Every interior slide pins the official DOE Office of Science seal and wordmark (`#828282`) at the bottom-left (`x = 60px, y = 1000px`), optional presentation/source context in the center, and the date + vertical separator + slide number (`#707276`) at the bottom-right.

## Graphic system

- **Signature mark: the ARM horizon wordmark.** The official lowercase `"arm"` geometric stencil paired with its curved planetary horizon arc (`viewBox="972 36 140 50"`, inline SVG in pure `#FFFFFF`), anchored at the top-right of every slide's cloud banner.
- **Surface: the binary-cloud atmospheric banner.** Sourced directly from the official template (`cached-gradients/sky.jpg`, `green.jpg`, `purple.jpg`, `navy.jpg`, `gray.jpg`, `split.jpg`), blending cumulus cloud photography with subtle binary telemetry (`0110100...`) across the sky.
- **Structural devices: the 9-National-Laboratory partner bar, DOE Office of Science seal, and ARM diamond markers.** Cover and closing slides carry the `#194173` navy partner bar showcasing the nine DOE national laboratories (Argonne, Brookhaven, Los Alamos, Berkeley Lab, Lawrence Livermore, NREL, Oak Ridge, Pacific Northwest, Sandia). Interior lists use the custom ARM rotated blue diamond (`::before` in `#0070C1`) for primary items and right-pointing chevron for sub-items.
- **Depth moment: the diagonal atmospheric split.** On `section-split`, an angled plane (`108deg` / `split.jpg`) divides the light-blue sky field from the deep-navy (`#194173`) exhibit stage.

## Density

`cover`, `section-divider`, and `closing` run `editorial`. `standard`, `section-split`, `comparison`, `picture-caption`, `metrics`, `architecture`, and `roadmap` run `balanced`. `time-series`, `bar-analysis`, and `instrument-table` run `data-dense`. Body copy stays between `16px` and `20px`; labels and footer metadata never drop below `14px`.

## Style anchors

- Official U.S. DOE ARM User Facility widescreen PowerPoint master (`arm-pptx-template.pptx`)
- ARM Mobile Facility (AMF) & Southern Great Plains (SGP) campaign readiness briefings
- DOE Office of Science Biological and Environmental Research (BER) program reviews
- Atmospheric System Research (ASR) working group keynote slides
- National Laboratory multi-institutional instrument specification dossiers
