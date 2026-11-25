# ARM User Facility — Layout Grammar

## Slide Types

| slide-type | family | visual roles | when | required slots | optional slots |
|---|---|---|---|---|---|
| `cover` | cover | `signature-mark`, `visual-plate` | opening title slide (`slideLayout1`..`5`) with 9-Lab bar and DOE footer | `title`, `presenter`, `organization`, `event`, `date` | `kicker`, `footer-label`, `theme` |
| `section-divider` | statement | `signature-mark`, `oversized-number` | full-bleed section divider slide (`slideLayout38`..`42`) | `section-no`, `title`, `subtitle`, `date` | `footer-label`, `theme` |
| `section-split` | split-visual | `visual-plate`, `item-marker` | diagonal split section or feature slide with image frame (`slideLayout31`..`37`) | `title`, `lead`, `h1-title`, `h1-body`, `h2-title`, `h2-body`, `h3-title`, `h3-body`, `figure-caption`, `date` | `eyebrow`, `footer-label` |
| `standard` | flow-diagram | `item-marker`, `signature-mark` | standard ARM content slide (`slideLayout6`) with four structured points and takeaway band | `title`, `lead`, `s1-title`, `s1-body`, `s2-title`, `s2-body`, `s3-title`, `s3-body`, `s4-title`, `s4-body`, `takeaway`, `date` | `eyebrow`, `footer-label`, `s1-meta`, `s2-meta`, `s3-meta`, `s4-meta` |
| `comparison` | comparison | `visual-plate`, `item-marker` | two-column comparison with `#0070C1` header bars (`slideLayout7` & `slideLayout8`) | `title`, `left-title`, `left-tag`, `left-items`, `right-title`, `right-tag`, `right-items`, `takeaway`, `date` | `eyebrow`, `footer-label` |
| `picture-caption` | image-spread | `visual-plate`, `oversized-number` | visual exhibit / picture with caption and observation metrics (`slideLayout9`) | `title`, `figure-caption`, `caption-title`, `caption-body`, `m1-value`, `m1-label`, `m2-value`, `m2-label`, `m3-value`, `m3-label`, `date` | `eyebrow`, `footer-label`, `site-code` |
| `metrics` | metric-hero | `oversized-number`, `item-marker` | hero campaign/facility metric with 2x2 supporting sensor KPIs | `title`, `hero-value`, `hero-unit`, `hero-label`, `hero-context`, `k1-value`, `k1-label`, `k1-note`, `k2-value`, `k2-label`, `k2-note`, `k3-value`, `k3-label`, `k3-note`, `k4-value`, `k4-label`, `k4-note`, `date` | `eyebrow`, `footer-label` |
| `time-series` | split-visual | `chartlet`, `item-marker` | atmospheric time-series or profile line chart beside diagnostic readout | `title`, `chart-title`, `chart-data`, `chart-labels`, `finding-title`, `finding-body`, `f1-label`, `f1-value`, `f2-label`, `f2-value`, `f3-label`, `f3-value`, `date` | `eyebrow`, `footer-label`, `chart-unit`, `chart-note`, `compare-data`, `compare-label`, `primary-label` |
| `bar-analysis` | cards-grid | `chartlet`, `item-marker` | comparative bar chart exhibit with three diagnostic finding cards | `title`, `chart-title`, `chart-data`, `chart-labels`, `c1-title`, `c1-stat`, `c1-body`, `c2-title`, `c2-stat`, `c2-body`, `c3-title`, `c3-stat`, `c3-body`, `date` | `eyebrow`, `footer-label`, `chart-unit`, `chart-highlight`, `chart-note` |
| `instrument-table` | table | `chartlet`, `item-marker` | instrument, site, or VAP specification table with synthesis band | `title`, `lead`, `row-headers`, `col-headers`, `cells`, `takeaway`, `date` | `eyebrow`, `footer-label` |
| `architecture` | matrix | `visual-plate`, `item-marker` | three-tier data pipeline or observatory architecture with facility rail | `title`, `rail-label`, `rail-title`, `rail-sub`, `t1-code`, `t1-name`, `t1-a`, `t1-b`, `t1-c`, `t2-code`, `t2-name`, `t2-a`, `t2-b`, `t2-c`, `t3-code`, `t3-name`, `t3-a`, `t3-b`, `t3-c`, `date` | `eyebrow`, `footer-label` |
| `roadmap` | timeline | `item-marker`, `visual-plate` | three-phase campaign schedule or multi-year deployment timeline | `title`, `p1-code`, `p1-name`, `p1-items`, `p2-code`, `p2-name`, `p2-items`, `p3-code`, `p3-name`, `p3-items`, `takeaway`, `date` | `eyebrow`, `footer-label` |
| `closing` | closing | `signature-mark`, `visual-plate` | closing summary, BER/ARM acknowledgment, 9-Lab bar, and contact details | `title`, `subtitle`, `acknowledgment`, `contact-name`, `contact-email`, `date` | `kicker`, `footer-label`, `theme` |

## Composition Rules

- First slide is always `cover`; last slide is always `closing`.
- Every interior content slide carries the official 176px ARM binary-cloud sky banner at the top (with bold white title on the left and the white ARM horizon wordmark on the right) and the DOE Office of Science footer at the bottom.
- Use `section-divider` or `section-split` to introduce major transitions in decks of 8 or more slides.
- Do not place more than 2 consecutive `data-dense` slides (`time-series`, `bar-analysis`, `instrument-table`) without an intervening `balanced` or `editorial` slide.
- `theme` slot on `cover`, `section-divider`, and `closing` accepts `sky` (default Light Blue), `green`, `purple`, `navy` (Dark Blue), or `gray` to match the five official ARM template color themes.
- Never fabricate real observatory photographs or field personnel; use `picture-caption` or `section-split` placeholder frames for user-supplied campaign imagery.
