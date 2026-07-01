# SCRIPT.md — decade-lens

Narration backbone. Durations derive from narration length, per the KB workflow
(`intelligence/techniques/hyperframes-from-website.md`, step 3).

> **VO/TTS: pending** (skipped in the first lint-clean build per workflow step 5).
> The draft narration table below preserves the full sourced prose, but it does NOT all fit
> the beat windows at a real read pace — use the **VO cut** below for recording/TTS instead.

Every factual line is sourced from the KB — no invented claims.

## VO cut — timed for the 50s composition (~156 wpm / 2.6 words-per-second)

Nine clips. `start` is where the clip begins on the master 50s track; `max end` is the hard
ceiling (next clip's start minus a breath). A clip may spill ≤0.5s past its beat's visual
cut — audio flowing across a cut is fine; two clips overlapping is not. If a generated clip
runs long, prefer trimming words over speeding playback.

| # | start | max end | Line |
|---|---|---|---|
| 1 | 0.5 | 6.3 | Twenty-thirteen. A three-hundred-dollar headset, and Alex teaching himself to wire Unity to it. |
| 2 | 6.4 | 13.0 | Twenty-sixteen. Josh calls Alex in first: "Let me pay forward what Jules Fisher did for me." |
| 3 | 13.2 | 17.6 | We craft real and virtual spaces — and the spectacles within them. |
| 4 | 18.6 | 25.4 | Ten years teach hard lessons: the cost of being wanted; require a deposit; protect "we're not sure yet." |
| 5 | 25.6 | 32.1 | One burned-out ask — a month of R&D, paid up front — and a freelancer becomes a studio. |
| 6 | 32.4 | 38.5 | Client work funds R&D. R&D becomes IP. IP wins the next client. |
| 7 | 41.8 | 43.4 | Ten years. Ten lessons. |
| 8 | 44.2 | 46.6 | Still bootstrapped. Still specialist. Still inbound-only. |
| 9 | 46.9 | 49.6 | Every three years, everything changes. Ship anyway. |

Speak "R&D" as "R and D". Clip 2's quote is Josh Dachs's pitch as recorded (paraphrased) in
the KB. Beats 1 and 7 lead with silence by design — let the headset draw and the ring draw
breathe.

| Beat | Window | Narration (draft VO) | KB source |
|---|---|---|---|
| 1 — Origin | 0.0–6.0 | It starts with a three-hundred-dollar dev kit. An Oculus Rift DK1 lands at Fisher-Dachs Associates, and Alex Coulombe teaches himself C# to wire Unity to it. | `context/business/overview.md` §2013 |
| 2 — Founding | 6.0–12.0 | In 2016, Josh Dachs calls Alex into his office — before Alex can ask. "Let me pay forward what Jules Fisher did for me." Agile Lens is founded. | `context/business/overview.md` §2016 (Josh's pitch, paraphrased on the record) |
| 3 — The craft | 12.0–18.0 | We craft real and virtual spaces — and the spectacles within them. Holodeck Anywhere. Blueprint Immersive. Stage Presence. Floor Tour. | tagline: overview.md §Identity (Alex, March 2026); products: `context/business/product-lines.md` |
| 4 — Lessons | 18.0–25.0 | Ten years teach hard lessons. Being sought-after is a blessing and a curse. Require a deposit — before you build. Protect time for "we're not sure yet." | `projects/harvardxr-keynote/overview.md` — lessons #3 (2018), #6 (2021), #7 (2022), exact talk titles |
| 5 — The turn | 25.0–31.0 | November 2022. Burned out, Alex asks for something new: a month of R&D, paid up front. The client says yes. The retainer funds the first full-time hire — and Alex-plus-contractors becomes a studio. | `context/business/overview.md` §Nov 2022 (retainer amount omitted per KB financial policy) |
| 6 — Flywheel | 31.0–37.0 | Client work funds R&D. R&D becomes IP. IP wins the next client. Disney. CBS. Kennedy Center. Four Seasons. The Royal Shakespeare Company. Waldorf Astoria. Dell. | overview.md §2023 (AI Dickens flywheel), §Notable Clients |
| 7 — Constellation | 37.0–43.5 | Ten years. Ten lessons. | keynote map finale (`projects/harvardxr-keynote/overview.md`) |
| 8 — Close | 43.5–50.0 | Still bootstrapped. Still specialist. Still inbound-only. Every three years, everything changes. Ship anyway. Agile Lens. 2016 to 2026. | overview.md §Present; bonus lesson: keynote overview |

Total: 50.0s.
