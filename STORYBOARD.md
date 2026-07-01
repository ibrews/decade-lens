# STORYBOARD.md — decade-lens

Per-beat direction. All beats typographic + SVG line-art (no raster assets — KB is
markdown-only and this repo ships self-contained; asset audit below).

| Beat | Window | Tag (teal pill) | Direction |
|---|---|---|---|
| 1 | 0/6 | ORIGIN · 2013 | Black. Wireframe DK1 headset draws itself in (stroke-dashoffset, 3 paths + magenta lens glint). H1 rises: "It starts with a $300 dev kit." Sub fades under. |
| 2 | 6/6 | FOUNDING · 2016 | H1: "Josh calls Alex in — before Alex can ask." Indented quote in gradient text: "Let me pay forward what Jules Fisher did for me." Sub: founded with Josh Dachs as co-founder, mentorship lineage. |
| 3 | 12/6 | THE CRAFT | Tagline hero, magenta aura pulsing softly behind (finite yoyo on a dedicated aura child). Four product chips stagger in (teal-border pills). |
| 4 | 18/7 | LESSONS, THE HARD WAY | Sub-tag cites the keynote: "from '10 Lessons from 10 Years' — HarvardXR 2026." Three lesson rows stagger in: year chip (keynote accent color) + lesson title. |
| 5 | 25/6 | THE TURN · NOVEMBER 2022 | H1 on the retainer ask; sub lands the punch: "…Alex-plus-contractors becomes a studio." |
| 6 | 31/6 | THE FLYWHEEL | H1 triptych: "Client work funds R&D. R&D becomes IP. IP wins the next client." Client marquee in two muted letterspaced lines. |
| 7 | 37/6.5 | (none — full-frame art) | Monocle constellation: ring draws clockwise, 10 year-dots pop in sequence (keynote accent rotation), cord drops from 3 o'clock to a '26 bonus dot. Center: "TEN YEARS / TEN LESSONS." |
| 8 | 43.5/6.5 | (none) | "Still bootstrapped. Still specialist. Still inbound-only." → bonus lesson in gradient: "Every three years, everything changes. Ship anyway." → lens-ring wordmark: AGILE LENS · 2016–2026. Holds to final frame. |

## Asset audit

| Asset | Type | Status |
|---|---|---|
| DK1 wireframe headset | inline SVG | authored in index.html |
| Monocle constellation | inline SVG | authored in index.html |
| Lens-ring wordmark motif | inline SVG | authored in index.html |
| Fonts (Manrope 200–800) | Google Fonts CDN | per KB findings: CDN fonts render correctly; bundle locally if FOUT appears in render |
| GSAP 3.12.x | cdnjs | standard |
| Raster images | — | none used (deliberate) |
| Audio | — | skipped with VO (SCRIPT.md) |
