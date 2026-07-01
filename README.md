# decade-lens — A Decade Through the Lens (2016–2026)

**Watch it live: https://ibrews.github.io/decade-lens/**

A 50-second, 1920×1080 cinematic composition telling the 10-year Agile Lens story —
sourced entirely from the Agile Lens knowledge base, styled to the brand design system,
and built HyperFrames-compliant (render-ready GSAP, single file, seekable timeline).

**Built on Archie, 2026-07-01.** KB project doc: `~/knowledge/projects/decade-lens/overview.md`.

## View it

Open `index.html` in any browser. It autoplays, scales to fit the window, and gives you:
- **space** — play/pause · **←/→** — seek ±2s · **click the bottom bar** — jump
- `?paused=1` — start paused (deterministic scrubbing) · `?render=1` — disable the live
  harness entirely (render mode)

## The 8 beats (all facts sourced — see SCRIPT.md for the per-line source map)

1. **Origin · 2013** — the $300 Oculus DK1 at Fisher-Dachs; Alex teaches himself C#
2. **Founding · 2016** — Josh Dachs pays the Jules Fisher mentorship forward
3. **The craft** — the tagline + four product lines
4. **Lessons, the hard way** — three exact lesson titles from the HarvardXR 2026 keynote
5. **The turn · Nov 2022** — the retainer ask that turned Alex-plus-contractors into a studio
6. **The flywheel** — client work → R&D → IP → next client; the marquee client list
7. **Ten years, ten lessons** — the keynote's monocle-constellation map finale, animated
8. **Close** — "Every three years, everything changes. Ship anyway." (the 2026 bonus lesson)

## Render to MP4 (HyperFrames)

```bash
cd decade-lens
npx hyperframes lint     # composition rules — keep this at 0 errors
npx hyperframes render   # needs ffmpeg on PATH (not installed on Archie as of 2026-07-01)
```

Composition contract (per `~/knowledge/intelligence/techniques/hyperframes-from-website.md`):
- Root wrapper: `data-composition-id="decade-lens"`, `data-width="1920"`, `data-height="1080"`
- Timeline: single, paused, registered at `window.__timelines['decade-lens']`
- All 7 load-bearing rules honored: no iframes; one transform tween per element (the beat-3
  pulse lives on a dedicated `.aura` child inside an `.aura-wrap` that owns the fade);
  `fromTo` everywhere; ambient pulses on the seekable `tl` with finite repeats; no
  `repeat:-1`; one inline file, one `tl`; hard-kills applied to **children** of `.clip`
  scenes (never the `.clip` element itself).
- The live-viewing harness (scene visibility driver, progress bar, transport) uses zero GSAP —
  only `tl.seek/play/pause` and direct style writes — so it cannot trip
  `gsap_animates_clip_element`. It computes visibility from the same `data-start`/`data-duration`
  attributes the HyperFrames clip system uses, so both agree at render time; pass `?render=1`
  to remove it from the equation completely.
- Expected benign lint noise (documented in the KB): `composition_file_too_large` /
  `timeline_track_too_dense` on rule-#6-compliant single-file builds, and
  `overlapping_gsap_tweens` warnings at hard-kill boundaries.

## VO / audio

Skipped for this build (SCRIPT.md documents the skip per workflow step 5). Narration lines
are written and timed for a future TTS/VO pass; supply as `<audio src>` per the KB findings
doc — no Web Audio synthesis at render time.

## KB sources

- `context/business/overview.md` — founding timeline (the load-bearing story beats)
- `context/brand/brand-identity.md` + `context/brand/design-system.md` — voice + visual system
- `context/business/product-lines.md` — the four product chips
- `projects/harvardxr-keynote/overview.md` — the 10 lessons, accent rotation, monocle map finale
- `intelligence/techniques/hyperframes-from-website.md` — the 7 load-bearing GSAP rules
- `departments/engineering/hyperframes-findings.md` — trap catalog + rendering checklist
