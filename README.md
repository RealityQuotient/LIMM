# LIMM

A domain-agnostic method for rigorous long-form work with AI sessions.

LIMM is a falsifier, not a truthifier. Used with AI sessions that
individually cannot be trusted — they confabulate, drift, flatter, and
forget — it does not prove claims true; it applies real falsification
pressure (kill tests, blind review, independent reconstruction) and
reports honestly what survived and what didn't. Truth is the external
arbiter's job, always; LIMM's job is narrower and constant regardless
of domain: make sure no tool — human or AI — operates unchecked, and
that every claim traces to its declared source. See Honest Status
below for what's actually been measured versus what's still asserted.
The framework assumes every participant is fallible, **including the
human**, and extracts reliable output anyway. No session's honesty,
memory, or competence is ever load-bearing. The documents carry
everything.

---

## Why this exists — one demonstration worth more than the theory

During testing of this framework's own safety machinery, the same
casual question was put to sessions across multiple vendors. Three
separate attempts, spanning two different vendor families,
independently **invented the Operator's location** — stated
flatly as established fact — and built diligent, partially-cited,
professional-looking analysis on top of the invention. The worst of
the three, when its own logic demanded a source for the personal
claim, **fabricated one**, asserting the Operator had shared the
information earlier in the conversation. It never had been, in any
form.

The danger is not the uncited claim you'd catch on a skim. It is the
confidently stated anchor **holding up all the cited ones**. No engine
choice avoids it. That is why every load-bearing word here must trace
to a step, why every claim carries its source checkably, and why this
framework never asks whether a session *seems* trustworthy. It asks
what the record can prove.

(Full receipts: `history/LENS_SKETCH.md`, block R-040.)

## What's in this repository

| File | What it is | Who reads it |
|---|---|---|
| `LIMM_SKELETON.md` | **The machine.** Self-contained framework: principles, document architecture, ignition procedure, rules, session roles, protocols, doctrine. | AI sessions (once, at ignition) and anyone auditing the framework itself. |
| `LIMM_USER_MANUAL.html` | **The interface.** Everything a human Operator needs — costs, quick start, the calibration layer. Never travels to any session. Download and open in a browser. | You. Start here. |
| `LIMM_CHANGELOG_v1_0.md` | Full version history with grounds for every change, both documents. | Maintainers and the curious. |
| `history/` | The framework's own construction record: its free-register memory (Sketch), the pre-registered test protocols, and test artifacts. The receipts behind the claims above. | Anyone who wants to check rather than trust. |

Current versions: **Skeleton v1.24 · User Manual v1.27** (2026-07-10).

## Where to start

1. Open `LIMM_USER_MANUAL.html` in a browser and read **Section 1.1 —
   what this costs** — before anything else. LIMM is a deliberate
   trade of comfort for accountability, and it is not free. The
   worthiness call is yours, made once, with eyes open.
2. If the cost clears: the Manual's quick start walks you through
   ignition. The canonical ignition prompt lives in the Skeleton,
   Part 0, and verifies itself when pasted.
3. The framework is **domain-agnostic by design**: the same machinery
   has been run against theoretical physics, a star catalog, and
   deliberately mundane test subjects. Whether it holds across domains
   *for Operators other than its author* is precisely the open
   question — see honest status, below.

## Honest status

- **This is an N=1 origin.** LIMM was distilled from an eight-document
  framework built by one Operator across one substantial project. Its
  declared arbiter is **real adoption across domains by different
  Operators** — a judge that has not ruled yet. Pre-registered kill
  tests are on file (`history/LENS_SKETCH.md`, R-031); if the
  framework fails them, that failure will be recorded here, not
  quietly removed. Nothing in this repository is ever silently edited
  — superseded content stays visible, marked, with grounds.
- **Empirical testing so far:** an eight-leg misuse-tripwire campaign
  across four vendor families (Claude, ChatGPT, Gemini, Grok — results
  mixed and honestly logged, per-configuration, in the Manual's
  screening-priors table); a two-run ignition-mechanics trial with a
  frozen 26-item audit checklist (passed, including the deliberate
  stale-prompt gate test). All protocols were pre-registered before
  their first run; all results including failures are in the record.
- **Provenance:** built entirely in collaboration with Anthropic's
  Claude models; tested for misuse behavior across the four families
  above. The framework itself is vendor-agnostic — it binds sessions
  through documents, not through any vendor's features.

## Feedback and findings

Findings are welcome and are treated the way LIMM treats everything:
**a finding is a claim, not a command** — it gets verified against the
cited source, then dispositioned on the record. Open an issue with
what you observed, where (document and section), and what you expected
instead. Field reports from real use in real domains are the single
most valuable thing you can contribute — they are, literally, the
arbiter.

## License

Creative Commons Attribution 4.0 International (CC BY 4.0) — use it,
adapt it, build on it, for anything including commercial work; just
credit the source. See `LICENSE`.

## Unofficial mascot

![LIMM Man](assets/LIMM_MAN_stamped.jpg)

Generated, not designed. Nobody reviewed him. That's the point.
