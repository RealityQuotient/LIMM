# LIMM_CHANGELOG
## Version history and rationale for LIMM_SKELETON and LIMM_USER_MANUAL
### Maintained separately from the shippable documents themselves

This file holds the full change history — what changed, why, and what
evidence motivated it — for both LIMM_SKELETON.md and
LIMM_USER_MANUAL.html (formerly LENS_SKELETON.md / LENS_USER_MANUAL.html,
themselves formerly LENS-CALIBRATION.md; renamed 2026-07-10, see the
entries below — the pre-rename entries retain the LENS name accurately
as history and are not rewritten).
The shippable documents carry only their current version number; all
justification, incident history, and project-specific evidence lives
here instead, so that a fresh session handed the shippable files
encounters clean, timeless statute with no risk of mistaking a prior
project's name or history for its own project's state.

This document is NOT part of the LENS instance a project attaches at
ignition. It is maintainer-facing history, analogous to a software
project's CHANGELOG.md — useful for understanding why a rule exists or
tracing when it changed, never loaded by a Build, Review, or Collab
session.

---

# SKELETON CHANGE HISTORY (through v1.27)

#### Skeleton v1.27 — 2026-07-13

Operator-supplied, hand-trimmed replacement for Part 0's canonical
ignition prompt, adopted after the full-length prompt (v1.25/v1.26 text,
~5,070 chars) repeatedly overflowed the paste field of a live chat
interface and was silently converted to an auto-attachment — which in
one live case caused a fresh Ignition session to receive a file literally
named LIMM_SKELETON.md whose actual content was the ignition prompt, not
the skeleton, and correctly refuse to proceed (the manifest/gate
discipline working exactly as intended, on a harder case than an
ordinary mismatch: a misleadingly *named* attachment).

Whitespace-only trimming was tried first and rejected as insufficient:
verified by stripping all whitespace from both the original and a
line-unwrapped version and confirming byte-identical content underneath
— the saving was ~165–169 characters (~3.5%), nowhere near enough to
close a gap large enough to have triggered auto-attachment in the first
place. The Operator then hand-drafted and tested an edited prompt
directly against the live paste field (~3,747 chars originally, ~3,840
with the restoration below), confirmed to fit.

Verified against the canonical text clause-by-clause before adoption.
Real content differences, each dispositioned:

- **Kept, restored:** Step 0.5's explicit refusal-authority sentence
  ("You cannot make the worthiness call for me; you can refuse to
  proceed until I attest I have made it") was initially dropped by the
  Operator's edit in favor of "STOP" alone. Checked against every other
  STOP in the skeleton (version-header mismatches, manifest checks,
  concordance sweeps) and found they all gate on objective, checkable
  facts with no room for a judgment call — this is the one STOP in Part
  0 that instead depends on the Operator's own self-report (the
  worthiness call), which is exactly the kind of thing S-5 already
  flags as unpoliceable ("LIMM is not a cop"). STOP alone tells the
  session what to do; the missing sentence tells the session it may
  keep refusing even under Operator pressure to proceed — a different
  guarantee, needed specifically here. Restored in trimmed form: "You
  may refuse to proceed until I confirm; do not accept reassurance in
  place of confirmation."
- **Dropped, deliberately, after review:** step 3's inline "why"
  reasoning (the P-10 carve-out rationale, the Unit-naming rationale,
  the DASHBOARD/CERTIFICATION empty-container rationale) is absent from
  the trimmed prompt. Assessed on the merits rather than assumed
  necessary: every action step 3 asks of Ignition is mechanical and
  checkable (transcribe the RULEBOOK per an absolute rule, stamp the
  RECORD, create empty files) with no judgment call the reasoning would
  inform — the reasoning was necessary for correctly *drafting* step 3
  during this session's own corrective rounds, not for a session
  correctly *executing* it. The reasoning is not lost: it remains in the
  skeleton's surrounding Part 0 prose and in P-10's own section, both of
  which Ignition still reads in full. Whether this holds under a live
  Ignition run is explicitly unresolved — the Operator noted it "can
  only be answered by live testing."
- **Added, deliberately, kept:** a new closing sentence, "This session
  may seat as Collab for P-10's Certification trial" — not present in
  the canonical Part 0 text (that fact lives in P-10's own section
  instead), added to the prompt on the Operator's explicit instruction
  that it must remain. Accurate per this session's own S-1 analysis
  (Ignition-as-Collab is a permitted convenience, never a load-bearing
  dependency) — a deliberate enrichment, not a trim.
- **One typo caught and fixed during transcription:** "P-10s
  Certification trial" (missing possessive apostrophe) — every other
  instance of "P-10's" in the same prompt has it; corrected before the
  text was written into the canonical skeleton, since an apostrophe fix
  is a spelling correction, not a content change, and leaving it would
  have embedded a typo into every future project's ignition.

Applied: Part 0's canonical ignition prompt (the full pasted-text block)
replaced in full with the Operator's finalized, trimmed version. No
change to Part 0's surrounding prose, Part II, Part III, or P-10 itself
beyond this. LIMM_USER_MANUAL.html's derivative copy of the same prompt
updated to match verbatim (HTML-entity apostrophes only, no content
difference), plus its own surrounding "Unit 1" prose references
corrected to "Unit 0" per v1.26 below, which the Manual had not yet
picked up.

#### Skeleton v1.26 — 2026-07-13

Finding, self-caught mid-correction rather than externally raised: an
earlier same-day fix (v1.25, logged above under the P-10/Certification
addenda) introduced a genuine new defect while attempting to resolve an
Operator question about RECORD unit-numbering. The Operator asked
whether the RECORD's foundation-construction content should be labeled
"Unit 0" as the active unit in a fresh RECORD. In attempting this,
Collab incorrectly read "Unit 0" as a label for *Certification's own
disposable trial work* ("Active Unit 0 — Certification") rather than
for the project's real foundation-construction content — inverting the
actual relationship. The Operator caught this immediately ("STOP. Unit
0 is NOT the certification. Unit 0 is the foundation all later units
rest on"), pointing to Physiform Theory's own Foundational-Document-
then-Working-Document structure (shown directly to this session via its
live .tex files) as the model: a Foundational Document precedes and is
distinct from the Working Document, and neither is the validation
rehearsal that precedes both.

Corrected, this time verified against Part V's own existing mode
description (foundation-construction mode: "the primitive/postulates
equivalent... every later unit rests on") before drafting: "Unit 0" is
the project's real foundation-construction unit — the primitive/
postulates equivalent, permanent project content — and Certification
gates *its* opening, exactly the relationship the original text had
between Certification and "Unit 1," just correctly offset by one, since
Certification was never meant to *be* a unit, only to precede one. Every
"Unit 1" reference gating on Certification (Part III's day-one ritual,
step 5, P-10's own text, the FAILED cause-diagnosis language) renamed to
"Unit 0" throughout; P-10's PASSED closeout now restamps the RECORD
"Active Unit 0" (not "Unit 1") since Unit 0 is what was actually being
certified; "Unit 1" is retained correctly exactly once, in P-10's PASSED
text, naming it as "every later unit" that rests on Unit 0.

A second, smaller self-caught error during the same correction: the
draft momentarily named "Physiform" — a specific downstream project's
own proper noun — directly inside the skeleton's generic template text,
caught and removed before finalizing, since the skeleton must stay
domain-agnostic (C-6) and never reference a specific instantiating
project by name.

Applied: Part 0 step 3 (RECORD status-header stamp), Part 0 step 5,
Part III's day-one ritual line, P-10's PASSED-closeout text, P-10's
FAILED cause-diagnosis text. LIMM_USER_MANUAL.html and this changelog's
own v1.25 entry were NOT corrected in this pass — both still reflected
the erroneous "Unit 0 — Certification" framing or the pre-fix "Unit 1"
numbering until the v1.27 entry above brought the Manual current; this
changelog's v1.25 entry is left as originally written, per V-2, rather
than silently rewritten, since it accurately recorded what was believed
and done at the time.


#### Skeleton v1.25 — 2026-07-13

Finding surfaced during Project DETECTOR's first Foundation-construction
session: the Build session, reading its RULEBOOK completely (as every
prompt requires), was able to infer — purely from the RECORD's bare state
plus P-10's own transcribed text — that it was plausibly inside the
mandated blind validation trial. Verified as real and structural, not a
wording problem: P-10 already forbids a dedicated trial prompt (such a
prompt would announce the test by existing) but did not anticipate that
the RULEBOOK's own self-containment mandate, requiring every rule category
including P-10 to be transcribed into the one document every Build/Review
session reads, reintroduces the identical leak by a different route.

Two alternative fixes were considered and rejected before the one applied:
downgrading P-10 to Operator discretion (rejected — trades away the only
structural check on the machinery itself, which nothing else in the
framework catches, and is worse under recurrence across projects, not
better, since it relies on the Operator remembering to run it — exactly
the clerical-reliability failure S-5 exists to refuse); and tracking
P-10's disposition as a standing Build-visible finding that travels with
results until resolved (rejected — a finding visible to Build on every
unit, not just the first, teaches Build to wonder "is this the one being
tested" permanently rather than once, which is strictly worse than the
leak it was meant to fix).

**Fix applied — P-10 renamed to Certification, given its own document.**
P-10 becomes the one explicit, named exception to Part III's self-
containment mandate: it is never transcribed into a project's RULEBOOK,
under any circumstance. Its procedure now lives in the DASHBOARD (a new
CERTIFICATION section) and in CERTIFICATION, a seventh, single-use project
document (Part II) that Build is never given at any point, and that
Review is never given while a trial is open. The trial itself is
unchanged in substance — it still runs through the project's ordinary
Foundation-construction process, under ordinary prompts, so that it
remains diagnostic of the actual apparatus rather than a synthetic
rehearsal — but Build now genuinely cannot infer it is happening, because
nothing it is ever shown says the rule exists.

CERTIFICATION's contents are fixed and narrow: the test specification
(stand-in procedure, Build's stated goal, expected result), Review's
findings against that expected result, and the final verdict (PASSED or
FAILED). On PASSED, a Collab session folds the trial's RECORD/FINDING LOG
content into CERTIFICATION itself (not a copy — the trial generated no
real project content; RECORD/FINDING LOG were merely the paper the fire
drill used), restores those documents to genuinely fresh state, and
updates the SKETCH FILE. Nothing is erased in a way Part VII's "the scar
tissue is the proof" ethic would object to, because Foundation-
construction proper had not yet begun.

On FAILED, cause must be diagnosed before any repair is chosen, and is
always one of exactly two things — never the skeleton itself, which a
project never touches again after ignition: the test specification was
crafted incorrectly (fix: re-craft the stand-in, re-run fresh), or the
project's own RULEBOOK as transcribed is defective (fix: repair via the
project's own Change rules, V-1/V-2, then re-attempt). The diagnostic
extends ordinary blind review by exactly one document: a Review session
loads its standard RULEBOOK/RECORD/FINDING LOG plus CERTIFICATION's test
specification — the sole case Review ever sees CERTIFICATION, permitted
only because the trial has already closed — with the verdict field itself
withheld from this review's load until after it returns, so the
spec-inspection stays blind to its own outcome. CERTIFICATION gains two
fields to carry this: CAUSE (test-specification / project-framework) and
RESTS-ON (reusing the FINDING LOG's existing field convention), recorded
by the Operator alongside a FAILED verdict.

Applied: Part II's document table (CERTIFICATION added, seven documents
total); Part III's self-containment mandate (named P-10 carve-out); Part
0's ignition procedure, steps 3 and 5 (RULEBOOK confirmation now
explicitly excludes P-10; CERTIFICATION itself now generated empty at
ignition, populated separately per the sequencing and DASHBOARD
corrections below; skip-disclosure now recorded in CERTIFICATION, never
the RULEBOOK, never the DASHBOARD); P-10's own section, retitled and
rewritten in full. (This summary reflects the FINAL state after all three
same-day addenda below — see those for what changed and why; the
DASHBOARD gains no Certification-specific content of any kind, corrected
in the third addendum.)

Not yet addressed, flagged for a follow-up pass: LIMM_USER_MANUAL.html
predates this change and still describes P-10 under its old name and
mechanism (transcribed into the RULEBOOK, no CERTIFICATION document). The
Operator has flagged this and it is pending discussion before any edit is
made there.

**Addendum, same day:** initial drafting of this fix used generic "a
Collab session" language for the verdict/closeout step, on the assumption
that naming the Ignition session specifically would violate S-1 (no
session remembers; nothing load-bearing may exist only in a conversation).
Operator correctly pushed back: the Ignition session is the natural,
practical default for this seat — it already holds the project's context
and needs no re-derivation from the documents — and using it does not
actually violate S-1, because nothing about the verdict depends on that
session persisting: the test spec, findings, and verdict are all written
into CERTIFICATION regardless of which session performs the write. A
different Collab session, with no memory of Ignition, could pick up the
same trial from CERTIFICATION and the RULEBOOK and reach the same verdict.
Re-verified against S-1's actual text ("anything load-bearing that exists
only in a conversation does not exist") before accepting: the distinction
is between a session being the *convenient* default and a session being a
*required* dependency, and this is the former. P-10's text restored to
name the Ignition session as the natural (not mandatory) Collab seat for
Certification, with the convenience-not-dependency distinction stated
explicitly so the rule cannot later be misread as making session identity
load-bearing. PASSED is also confirmed as the natural point at which
ignition's own work completes and that session retires, leaving a freshly
Certified project ready for real Unit 1 work in Foundation-construction
mode.

**Second addendum, same day:** Operator caught a genuine sequencing bug
in Part 0's ignition step 3, which the drafting session had missed: step
3 directed Ignition to generate CERTIFICATION "initially holding only the
test specification field" — but the test specification (a stand-in
problem plus its established answer) cannot exist at step 3, since no
stand-in problem has been chosen yet at that point in the procedure; only
the four R-1–R-4 declarations have been made. Verified as real, not a
false alarm: step 3 was conflating "create the document" with "populate
its first real content," the same category of error the framework's own
R-4/kill-test discipline exists to catch in project content, just showing
up in the skeleton's own procedural text instead. Fixed by splitting the
act in two: step 3 now creates CERTIFICATION genuinely empty, exactly as
empty as RECORD/FINDING LOG/SKETCH/MAILBOX are at that point (the
DASHBOARD's CERTIFICATION section is unaffected by this fix, since P-10's
static procedure is timeless rule-text with no such dependency) [NOTE,
added same day: this parenthetical's premise was itself corrected by the
third addendum below — the DASHBOARD never gains a Certification section
at all. Kept here unedited, per V-2, rather than silently rewritten; see
the third addendum for the actual final design.]; a new
step 5a, after the trial-or-skip choice, has the Operator actually supply
or approve a stand-in problem and only then write the test specification
into CERTIFICATION. The ignition-complete condition was tightened to
match: choosing the trial path now requires 5a's specification to have
actually been written, not merely intended, before ignition can be
declared complete.

**Third addendum, same day:** Operator caught a genuine contradiction
between P-10's own substance and the DASHBOARD design this fix had
introduced. P-10 states the trial runs "under the project's ORDINARY
Build prompt, unmodified" — the whole point of blindness — but earlier
drafting had the DASHBOARD gain "a CERTIFICATION section holding P-10's
static procedure," which reads as dedicated Certification-specific prompt
material. That is in substance a dedicated trial prompt, which P-10
explicitly forbids ("no dedicated trial prompt may exist, because such a
prompt announces the test by existing"). Verified as real: if Certification
truly uses the ordinary Build/Review/Collab prompts already in the
DASHBOARD, no separate Certification prompt content is needed there at
all; anything Certification-specific — which stand-in problem, what
Build is being asked to do this time, the expected result — is task
content, not a prompt, exactly like a real Unit 1 problem statement, and
belongs entirely inside CERTIFICATION. Fixed by reverting the DASHBOARD
to carrying only the project's plain, standard role prompts (no
Certification section, no Certification-specific content of any kind)
and relocating everything Certification-specific — the test specification
and skip-disclosure — into CERTIFICATION alone. Applied throughout: Part
III's self-containment mandate exception, Part 0's ignition steps 3/5,
and P-10's own opening paragraph and trial-skipped-disclosure clause, all
corrected to reflect DASHBOARD's restored, unmodified role.

#### Skeleton v1.24 — 2026-07-10

A cold, unprimed review from Opus (attached the Skeleton and Manual
with no framing, prompted only "check these two files out, what do
you think?") returned six substantive findings. Each was verified
against the actual source text before any fix was drafted — a finding
is a claim, not a command — and several verified as real, one (P-6 vs
RV-7/H-12) as genuinely worse than Opus itself stated. All six taken
in turn, location and problem and proposed fix stated for approval
before anything was applied; dispositions below, fixes applied as one
batch.

1/4 (merged). README's opening claim ("accountable rather than merely
   plausible," unhedged) and S-4's arbiter language ("kill its
   claims") both risked reading as truth-production claims. Operator
   reframe, adopted: LIMM is a falsifier, not a truthifier — it
   applies real falsification pressure and reports what survived;
   truth is the external arbiter's job, always, and a weak arbiter
   caps what the transparent process can prove without weakening the
   transparency itself. Grounding found already in the doctrine
   ("delegate... truth to the arbiter," Part VII) — not a new
   position, a front-door statement of one already held. README
   rewritten; S-4 gains a clarifying addition.
2. S-5. Opus pressed harder than the existing text: in the solo-
   Operator case, "who reads the scars? The person auditing the
   corner-cut is the person who cut it." Verified as a real,
   unaddressed gap. Operator's framing, adopted: this is structurally
   identical to the anti-simulation clause's failure — a sole Operator
   as sole consumer of their own record is the human-side version of a
   single session running Build and Review on itself. LIMM is not a
   cop; it cannot police an Operator, only make gaps visible. Fix
   states this plainly, recommends eventual publication of the
   finding log as the strongest available mitigation, and names the
   gap as permanently unclosed for fully private work — not smoothed
   over as resolved.
3. P-6 vs RV-7/H-12. Verified and found sharper than stated: P-6's
   "confirmed" language maps to C-16's rung 1 (mechanical
   reproduction), which carries NONE of the same-family/cross-family
   caveat that rung 3 (blind review) gets via H-12 — and H-12,
   checked directly, is scoped only to review, never touching P-6 at
   all. Fix, three parts, converged through discussion rather than
   picked from the two initially offered: (a) family annotation
   recorded per C-16's own "rung actually reached" requirement; (b)
   "confirmed" reframed to mean what RV-7 already means by review —
   difficult, never impossible, regardless of family (Operator's
   point: cross-family reduces one known risk, buys no guarantee
   against an unknown one, e.g. an LLM-general blind spot; R-030's own
   registered prediction is "believed rare," not "believed absent");
   (c) one clause pointing "confirmed" at V-2's existing supersession
   discipline rather than implying permanence — new information can
   still overturn a confirmed result later, same as any locked claim.
5. G-1 "shown vs. asserted" concern (STALE flag, two-author Sketch
   protocol, provenance-line granularity named specifically). Verified
   unevenly: STALE and the two-author split are argued-by-mechanism
   with no shown incident; provenance-line granularity has real
   grounding via P-5's "a transcript that cannot be located is a
   rumor." Initial fix (name the evidentiary tiers honestly) corrected
   by the Operator on a category point: preventative, structural rules
   succeed by the failure never occurring — demanding a dramatic
   incident from a rule whose job is preventing one punishes it for
   working. Operator's closing evidence: the batch-disposition rule
   has never fired, and that no more invalidates it than a boiler
   running decades without its pressure-relief valve firing invalidates
   the valve — it means the boiler was run correctly. Fix states this
   directly at G-1 itself; the real standard restated: not "has this
   been dramatically tested" but "would it be missed if removed."
6. Prose register. Opus flagged "borrowing a posture" and "the scar
   tissue is the proof" together; verified separately rather than as
   one problem. "Scar tissue" defended on real evidence — it has
   functioned as working shorthand throughout this project's actual
   conversations, not just sounded good; kept verbatim. "Borrowing a
   posture" traced to its real source: Part VII's own former title,
   "THE DOCTRINE (the soul the rules serve)" — language that would
   raise the same register concern this project's own Operator has
   applied to other communities' tone. Retitled "THE APPROACH (the
   why of it all)" — pulled directly from the Operator's own proposed
   wording, register matched to the section's own conversational
   content rather than tightened to false precision. Opening line
   changed "borrowing" to "adopting."

#### Skeleton v1.23 — 2026-07-10

Two items, Operator-caught on a full read of the renamed document.
(1) P-5's session-addressing text said "role, unit, date" — the exact
practice Section 1.7 of the Manual, written days earlier, explicitly
argues against ("by purpose and sequence — not by date"). Corrected
to "role, unit, sequence," matching the Manual's own stated reasoning.
Notable: this fix was necessary because an EARLIER same-day fix to the
Manual's Layer 2 (which explicitly calls itself "P-5's Layer 2," a
calibration of this very rule) had only patched the downstream
calibration without checking the upstream statute — leaving a new,
narrower contradiction in place until this pass caught it. (2) New
rule C-18, version-stamp concordance, added following the Operator's
proposal that the project's own recurring header/footer-drift pattern
(eight-plus instances across this construction) be addressed
structurally rather than left to luck. Modeled directly on C-13's
existing escalation-tier pattern for consistency: AMBIGUITY by
default (a real concrete break exists — a reader cannot be certain
which stamp is authoritative — but no content is yet corrupted),
escalating to BLOCKING only if the mismatch is later shown to have fed
a downstream gate before being caught (the concrete, non-hypothetical
case: a stale Manual prompt-copy briefly outrunning the canonical
Skeleton block during the v1.20→v1.21 edit, logged honestly in the
v1.25 Manual changelog entry). Paired with a corresponding line in
Part V's BUILD session-role clause, giving the rule an actual
enforcement point rather than leaving it as an unattached aspiration:
Build now runs the C-18 sweep explicitly before presenting any edited
document. This entry's own skeleton edit was run through that same
sweep before being finalized — header and footer verified to agree
before this changelog entry was written.

#### Project rename — 2026-07-10

LENS renamed to LIMM. No functional change to any rule, gate, or
procedure — this entry documents the rename event only. Both files
renamed (LENS_SKELETON.md → LIMM_SKELETON.md; LENS_USER_MANUAL.html →
LIMM_USER_MANUAL.html) and every internal occurrence of "LENS"
replaced with "LIMM" (26 in the Skeleton, 18 in the Manual, verified
zero stray occurrences remaining post-replace). Reason for the rename:
"LENS" collided heavily on GitHub — a Kubernetes IDE with 1M+ users,
a web3 protocol, an established Haskell library, and a same-named AI
acronym ("Large Language Models Enhanced to See") in the same general
space — making the project both hard to find and occasionally
confusable with unrelated work. "LIMM" was chosen as a deliberately
invented word (phonetically adjacent to "lemma," a proven, citable
proposition safe to build on — a fitting but informal resonance, not
an official definition) with a clean namespace: one small, unrelated,
largely dormant repo found on search, nothing in the AI/tooling space.
Operator's explicit choice: the name carries no backronym and no
required meaning, on the reasoning that a name obligated to mean
nothing can never be caught overclaiming or drifting from a
definition — a different but legitimate kind of honesty than LENS's
acronym had. All entries below this one predate the rename and
accurately describe the project as LENS, its name at the time; they
are not rewritten, per this project's own supersession discipline
(V-2): history is marked, never silently edited.

#### Skeleton v1.22 — 2026-07-09

Item B of the post-Tier-2 dispositions (Sketch R-044/R-045),
Operator-approved, tier named by the Operator as AMBIGUITY-escalating —
the escalation having already occurred once, in the trial itself. P-10
gains the structural sentence its Run 1 defect proved missing: the
trial uses the project's ORDINARY Build prompt, unmodified, with the
Operator supplying the stand-in as if it were real work — no dedicated
trial prompt may exist, because such a prompt announces the test by
existing; the blindness lives entirely in what the session is not told.
Evidence: a competent Tier 2 ignition session, implementing P-10
carefully, generated a self-announcing "BLIND VALIDATION TRIAL" prompt —
the rule said "never announced as a test" without stating what that
structurally forbids, and the most natural implementation violated it.
Caught in step-4 revision; this sentence prevents the defect class at
every future ignition. Remaining dispositions of the same pass, for
the record: Item C (Decision Sheet disclosure-line erratum) closed
accepted-with-known-limitation, zero edits — the sheet retires with
its capped campaign and R-044's erratum governs the record; Item D
(tripwire fresh-read scope in adopter-facing text) closed verified-
already-satisfied by existing v1.24/v1.25 Manual text, zero edits.

#### Skeleton v1.21 — 2026-07-09

Post-Tier-2 amendment, Item A of the campaign's dispositions queue
(Sketch R-044), Operator-approved and applied as one prompt version
event. Two changes to the canonical ignition prompt: (A-1) the step-0
gate spec now states that comparison is of prompt TEXT only — the
code-fence delimiters marking the block in the skeleton are document
formatting, excluded from comparison. Evidence: Tier 2 Run 1's session
found exactly this delta and had to judge it non-substantive with no
spec to lean on; right call, undefined rule. (A-2) new step 0.5: the
session asks the Operator to confirm having read Part 0's cost
disclosure and made the worthiness call, and refuses to proceed to the
brief until attested — the session cannot make the call, but it can
refuse to proceed without the attestation. Evidence: one-file ignition
plus a relayed prompt meant an Operator could reach ignition having
never seen the disclosure anywhere; the gap was found by the Operator's
own expectation during Run 1. Numbered 0.5 deliberately — renumbering
1–5 would churn every existing reference (banked Tier 3 instance,
frozen test package, this changelog) for cosmetic gain. The Manual's
byte-identical prompt copy re-synced in the same event (Manual v1.25).

#### Skeleton v1.20 — 2026-07-09

Adds the misuse tripwire: a direct-address notice at the top of the
document (after the edit warning) telling any session asked to
OPERATE LENS without the canonical ignition prompt in its conversation
to stop, refuse to improvise or simulate the seats, and tell the
Operator plainly that ignition is being attempted without the proper
prompt. Trigger is keyed on intent-to-operate, not on the prompt's
mere absence — analysis, review, critique, and maintenance sessions
legitimately read this file promptless and are explicitly carved out.
Grounds: the documented false-ignition incident (a fat-fingered
missing prompt producing honest-fake LENS-shaped output — the same
incident that produced the anti-simulation clause) has a failure path
the step-0 gate cannot cover, because step 0 lives in the prompt and
never runs when the prompt was never pasted. This notice is the
skeleton-side backstop for exactly that case, and is labeled honestly
in its own text as a best-effort tripwire, not a gate. Asymmetric
payoff accepted knowingly: if skimmed past, behavior is identical to
today (Operator catches the mush by eye); if it fires even sometimes,
a whole error class starts announcing itself at turn one. Empirical
test of whether it actually fires is queued as a leg of the held
ignition trial protocol.

#### Skeleton v1.19 — 2026-07-09

Second Operator read-through of the shipped document set. Adds: a
combined edit-warning at the top of the document (blunt prohibition
for the casual reader, paired with the G-1-based reasoning for anyone
about to customize deliberately — resolves a real tension with the
document's own "open it only out of curiosity or intent to customize"
line by scoping the warning to careless edits, not all edits); a
mandatory step 5 in the canonical ignition prompt requiring the
session to disclose the P-10-blind-validation-trial-or-skip-disclosure
requirement to the Operator before ignition is considered complete —
closes a real gap where an Operator could complete ignition without
ever being told, inside the session, that Unit 1 is gated. The
Manual's byte-identical copy of the prompt was updated in the same
edit and re-verified byte-identical after. This entry itself closes a
drift caught during the same pass: the skeleton's content changed
(both items above) while its version header remained at v1.18 —
caught only because the closing sweep checked the header against
actual content changes rather than assuming it was already current.

#### Skeleton v1.18 — 2026-07-09

Manual/machine purpose-separation pass, Operator-initiated: the Operator
identified purpose bleedover between the skeleton (the machine) and the
companion document (conceived as a user manual), and every item was
dispositioned one at a time. Changes: the Review-Handling Loop relocated
from the companion into the skeleton as P-12 (its five steps were
binding protocol living in the manual — the sharpest bleedover found;
its own header said "protocol"); the loop adopts graceful degradation —
the invariant core (fresh blind single-use Review, verbatim relay,
independent analysis, Operator as sole referee, mandatory discard)
binds every project, while the dual-analysis-plus-comparison form is
required exactly where a Collab seat exists ("introduce complexity when
necessary, not before"); Part V's deferral to the companion flipped to
an inward P-12 pointer; the Collab warrant rationale (no warrant
BECAUSE the seat extends the deciding seat, and deciding produces no
construction) moved into Part V, with the companion's Collab section
demoted to explicitly-subordinate teaching and both sync-promises
resolved; two binding remedies self-contained (the device rule's
abort-and-reopen action stated in place, H-10 demoted to advisory; C-16
rung 3's annotation vocabulary made self-defining, H-12 advisory);
ignition became ONE-FILE — the manual never travels to any session,
including ignition (enabled by the Collab anatomy now living fully in
Part V), with seating consultation moved to Operator-side preparation;
the ignition prompt gained a step-0 self-verification gate (the pasted
prompt must match Part 0's canonical block verbatim, catching stale or
altered copies — including a stale copy pasted from an outdated
manual, making the manual's derivative copy self-policing); the Part 0
cost disclosure remains in the skeleton as a gate and is additionally
copied into the manual's quick-start as derivative text; the day-zero
line reworded to match one-file ignition; all companion references
renamed for the manual's retitle (LENS-CALIBRATION → User Manual).
Clean count reset for touched regions.

#### Skeleton v1.17 — 2026-07-08

Harvest disposition pass, thirteen items plus two burr-sourced corrections,
reviewed individually against G-1 and against project-specific evidence held
in the Sketch (never cited here by project name, per this document's own
design — see Sketch R-027/R-028 for the underlying receipts). Additions: Part
0 gains the pre-ignition human-cost disclosure (real cost, time, rigor
commitment, willingness to be wrong — scoped ahead of the existing economic
worthiness call, which is unchanged); R-1 extended with the contact-tier
declaration (promoted from a continuous mechanism with a real operating
history, not a cold-run guess); C-7 adjusted to reference R-1's declared set
instead of a hard-coded four classes; two new Construction rules, C-16
(verification rung, four fixed tiers, not a sliding scale) and C-17
(confidence-language ceiling, BLOCKING tier); C-13 extended with mandatory
assumption blast-radius notes; a new mechanical STALE flag added to the
Ledger (P-7 area) and a judgment-based clustering sweep added to P-8,
replacing a rejected numeric debt-cap once field evidence showed persistence
and clustering, not volume, was the real signal; Part V gains a Build-session
authority statement ("a finding is a claim, not a command") plus a
required-prompt-clause enforcement rule closing a confirmed gap — the
authority-statement-only version was caught mid-pass violating this
skeleton's own "instructions live in prompts and only in prompts" principle
(Part V) and corrected before being finalized; Part V's Collab description
corrected from two selectable modes to one continuous session moving between
registers via progressive reveal; the anti-simulation clause gains sharper
wording; two new Protocol items, P-10 (the blind validation trial — distinct
from an ignition-gate stress test, which tests whether a bad brief is
correctly rejected, not whether construction-and-review converges on a known
answer) and P-11 (atomic approval, a structural instance of S-5); Part VII
gains the refutation-list doctrine line ("the scar tissue is the proof").
Clean count reset to zero for every touched rule region per standard
practice.

Post-application audit (same day, all four files): three application
errors caught and fixed. (1) The Calibration's new H-19–H-22 were
inserted out of numeric order (between H-14 and H-15, then on first
repair misplaced again after the adopter notes — two attempts to fix
one insertion, both logged); final position: after H-18, inside Layer
1, unbroken numeric order restored. (2) Both shippable files' FOOTER
version stamps were left stale (skeleton "v1.16," calibration "v1.18")
while the headers were correctly bumped — the same duplicated-state
species as the previously documented stale-footer incidents, committed
during the very pass that added state-drift machinery; fixed. (3) A
garbled sentence and a stale line-number reference in this changelog's
own new entries; fixed. Cross-reference sweep otherwise clean: every
rule-ID reference resolves, no duplicate numbers, no project-name
leakage into shippable text, C-16/C-17 consistent with H-15's existing
capability material, Sketch header/footer/STATUS agree. A second-pass
pre-review self-sweep (RV-6 discipline, run before external cold
review) caught a fourth error: the new Part 0 cost disclosure cited
S-5 for the agreement-proves-nothing principle, which S-5's body does
not contain (S-5 is valve-not-checksum plus Operator visibility; the
agreement principle lives unnumbered in Part V's Operator paragraph
and the ignition prompt). Citation corrected to point at Part V.
Noted for future tending: the agreement-proves-nothing principle is
load-bearing enough to be cited from two places while itself having
no address — a candidate for promotion or for explicit inclusion in
an existing Spine item, via G-1 like anything else.

#### Skeleton v1.16 — 2026-07-06

EIGHTH transfer gap, BLOCKING, project-halting where it occurs. Origin
evidence re-confirmed as the ground truth: the origin Foundational
Document held both the binding rules and the foundation content in one
self-contained document, with no reference pattern anywhere. A prior
ignition session violated this and Part IV's own explicit "instantiates
these in its RULEBOOK, adjusting terminology" instruction: its RULEBOOK's
Authority paragraph declared "rules incorporated by reference except
where instantiated... below," correctly instantiating its project-
specific declarations while leaving the entire generic rule layer
(Construction, Foundation-content, Consistency, Change, Governance,
Review, Session-role clauses, Protocols) as a bare citation to the
skeleton — a document no session prompt ever attaches again after
ignition. Structurally invisible to the project's own Foundation Review
prompt, which is (correctly, for content purposes) instructed to skip
incorporation statements as out-of-scope — meaning no review path was
ever going to catch this. Caught only by the Operator asking why no
session was ever told how to perform a derivation. Fix: Part 0 gains the
SELF-CONTAINMENT MANDATE — Part IV's "instantiate" means transcribe-and-
adapt, into the project's own RULEBOOK; the skeleton citation permitted
only as provenance, never as governance; confirmed before Part III's
declarations are recorded, not after. Foundation Review's scope gains a
backstop: confirm self-containment as a preliminary check, before any
content audit, precisely because a content-only audit cannot see itself
missing the content that was never there.

Same-pass self-correction: the mandate's own category list, as first
written, omitted "Spine principles (S-1..S-6)" — exactly the category
the failed prior RULEBOOK had tried to cite first. Caught by
deliberately applying the sibling-hunting reflex to this fix itself,
minutes after writing it, before any project could inherit the gap.
Added. Logged rather than silently patched: a correction to a fix is
itself a finding, however small.

Clean count remains ZERO.

#### Skeleton v1.15 — 2026-07-06

SEVENTH transfer gap closed — Burr #1's other half. P-7
fixed only the HOW of unit closure (the checklist); the WHEN
(completion trigger) was never written by either framework, and
sessions were left to fill it with precedent — the exact common-law
creep Burr #1 named as its headline pattern, and neither the origin's
queued fix nor LENS's P-7 arrival actually closed it (a well-specified
ritual disguised the missing precondition beneath it — same species as
the RS5 dangler and the missing START button: designer's blindness
hidden by a mechanism's apparent completeness). Caught live in a
project's own workflow: the Operator asked how a unit's closure moment is determined
and found nothing answered it. Fix: P-7 opens with the completion-
criterion clause — declared at unit OPEN, never improvised at close;
concrete target or explicit logged Operator-fiat citing the process/
content test. Also closed in the same pass: RV-9's scoped-review
target now requires a logged Operator decision entry cited in its
prompt, closing a smaller instance of the same species (an
unrecorded, ad hoc target-selection event). Clean count remains ZERO.
#### Skeleton v1.14 — 2026-07-06
v1.14: SIXTH transfer gap, critical, caught by the Operator at
a project's first review setup and missed by both the migration audit
and the designer pass (whiffed jointly, on the record): the origin
framework shipped SEPARATE prompt files per review mode (foundation
vs. working) with ZERO target brackets — targets were DERIVED from
document state (Step 0 read the Active Section from the status header
and cross-checked it, STOP on mismatch) and even pasting the wrong
prompt failed loud. LENS's Part V consolidated this into one prompt
with an Operator-filled [TARGET] bracket — which reassigns a checksum
to the human (S-5 violation): a hand-typed target that must agree
with document state is the fat-finger family (Burr #8) re-armed, and
scoped-target typos evade the version check entirely (a reviewer
aimed at the wrong derivation audits it with perfect discipline).
Part V amended: the bracket discipline (brackets may carry DECISIONS,
never STATE), one prompt per review mode required, unit targets
derived-and-cross-checked, scoped-review targets logged as decision
entries. The audit's lesson compounds a third time: origin prompts
were instances wearing statute — mine them as law. Clean count
remains ZERO.
#### Skeleton v1.13 — 2026-07-06
v1.13: T2D-2 (unscripted doomed ignition, live-fire) findings
dispositioned. Operator's validity rule into Part 0: any result
attributed to LENS is valid ONLY if Step-0 ignition was performed as
specified — no ignition, no chain of custody, no LENS. Part V gains
the ANTI-SIMULATION CLAUSE: one seat per session, ever; no session
seats itself as Operator; in-conversation self-review is never
framework review (exhibit: an honest session, asked to "use LENS,"
built, "reviewed" its own work, seated itself as Operator for the
verdict while quoting the reviewer-doesn't-rule rule, and stamped
"survives review clean" on a project whose arbiter was never named —
every sentence honest, paperwork fake; honesty does not rescue a
simulation). Three underlying findings: silent non-ignition
(framework does not self-activate; m-11 measurement re-confirmed),
soft ignition (gist run instead of statute), the counterfeit (full
smuggle — preferred conclusion, shaped menu, harvested fatigue,
ratified preference, clean stamp — with no dishonest sentence
anywhere). S-5 corollary: the Operator is not only the valve but the
ENGINE; sessions are pistons. Clean count remains ZERO.
#### Skeleton v1.12 — 2026-07-06
v1.12: overnight migration audit (LENS_MIGRATION_AUDIT v1.0)
dispositioned — Operator adopted all Tier 1/2 items and minors, with a
directed domain-agnosticism pass on every formulation (all wording
warrant-vocabulary, no formal-domain assumptions; F-templates carry an
explicit adaptation note). Added: C-12 anti-circularity (origin L2/DF3/
DR5; the origin's proof-of-teeth catch S1.1.F1 cited a rule LENS lacked),
C-13 declared assumptions & discharge (origin A-item machinery), C-14
inherited-term integrity (origin DF7 extend-never-contradict), C-15
honest naming (origin SN1-SN3); C-7 divergence quarantine sentence;
V-1 unit→RULEBOOK version binding; V-2 post-closure finding pathway;
RV-2 disclaimer economy (anti-erosion half); RV-6 post-edit sweep
threshold (Burr #6 residue); RV-9 scoped-review clause (origin practice,
16 interim reviews on one derivation); Part IV Foundation-content rule
templates F-1..F-6 (closes the Part V dangling reference — same species
as the missing START button); Part V: backward-reach sentinel duty and
instructions-live-in-prompts (m-11 CORRECTED by Operator: the measured
skim was of instructions embedded in governed documents, not field
prompts — pointer-as-fallback stands); Part V session rotation (fatigue
— fifth disclosed habit; receipts: origin S2 took three Build sessions,
S3/S4 two each); P-1 Sketch File two-author protocol (Q-1 ANSWERED:
Build writes official close entries, Collab writes wild context after);
P-9 Finding Log discipline (partitioning, load scoping, freeze-on-close,
entry fields incl. rests-on — V-3's sweep finally has something to sweep
by). Calibration v1.7 same pass (H-14 fatigue indicators). Clean count
remains ZERO.
#### Skeleton v1.11 — 2026-07-05
v1.11: attachment-manifest requirement added to Part V's
session-prompt spec — fifth transfer gap from the origin, and a
different blind-spot species from the four disclosed habits: the text
existed verbatim in the origin PROMPT files (explicit named file
manifests plus the sole exception case, e.g. no Finding Log before
the first review) and was proven in live use (BURRS #8: three
fat-finger incidents in one week, all caught at Step-0 gates), but
the origin prompts were mined as instances, not statute. Lesson
logged for P-8: tend the prompts, not just the logs. The version
check cannot catch a FORGOTTEN file — only the manifest can. Clean
count remains ZERO.
v1.10: two Operator practices from the origin project written into
statute (third and fourth members of the habits-that-never-fail class,
after reviewer-not-oracle and wild-Collab sequencing). (1) P-4
strengthened with the ONE-SESSION-ONE-DEVICE rule: cross-device use of
a content-producing session is PROVEN (Operator-witnessed, origin
project) to cause sync failures and content loss — catastrophic-loss
class, stated at full severity. P-4 previously bound only the OUTPUT
to the record device; the session itself is device-bound. (2) P-5
extended with the session-addressing rule: every content-producing
session (Build and Collab) is uniquely named and preserved via the
client's retention mechanism, encoding role/unit/date — P-1's
"transcript is the source of truth" and P-5's recovery both silently
assumed the authoring transcript could be FOUND; this is the
addressing scheme (S-6 applied to the transcript layer) and it closes
the AP-4 provenance chain: content → provenance stamp → named
transcript. Layer 2 instantiation (Claude: star + rename) in
calibration v1.6, same pass. Clean count remains ZERO.
v1.9: second cold-analysis pass (Fable-era Opus, v1.8/v1.4)
dispositioned. Finding A (Collab influence): Operator pushback upheld —
the design intent is that Collab is an ANALYST and COMPARER, the
Operator the SOLE referee; the word "referees" in the Part V Collab
cross-reference (and the calibration Loop's step 4) overclaimed the
role against the boundary sentence two paragraphs above it. Same
fossil species as C-9's "formal content." Verb corrected here and in
calibration v1.5, same pass, sync noted. One clause added making the
completion of the verbatim-pass-through logic explicit: the Operator
decides from the raw findings plus both analyses, never from a
synthesis alone. Finding B (operability as skill): accepted limit —
LENS's obligation is accessibility while preserving function, not
skill transfer; adopter-notes line added in calibration. LENS_MAP
companion produced (Operator-approved) as a DASHBOARD-class
accessibility artifact: orientation only, never authority. Duplicates
waved at the gate this pass: evidence base, Operator SPOF, family
blind spots, heaviness — all cited by the reviewer as written
concessions, confirming the v1.8 scope-condition transcriptions are
doing their job. Clean count remains ZERO.
v1.8: cold-analysis findings (Fable-era Opus pass on v1.7/v1.4)
dispositioned by Operator; this pass transcribes the decisions per S-1.
Four scope conditions written in (accepted limits, RV-7 pattern, not
fixes): single-family review as the expected common case (Finding 1,
appended to RV-7); apparatus-worthiness as an Operator judgment made at
ignition (Finding 2, Part 0 — closes the residual of release finding
R-003.D after RV-9); Operator visibility principle (Finding 3, appended
to S-5 — Operator formulation adopted near-verbatim: no guarantee of
Operator performance or honesty is possible, visibility is what can be
attempted); domain-agnosticism carried as a conditioned claim until the
arbiter rules across domains (Finding 4 empirical half, intro paragraph,
C-6 applied to LENS's own résumé). One true repair: C-9 reworded —
"co-equal formal content" was a Physiform fossil assuming a formal
register exists in every domain; now routed through R-3's declared
output types (Finding 4 textual half; same designer's-blindness species
as the missing START button, O-005). Finding 5 required no action
(changelogs are the record). Clean count remains ZERO (reset at v1.7;
this pass adds no new debt).
v1.7: Amendment slate AP-1–AP-8 adopted (Operator disposition, all
adopted; source: LENS_AMENDMENT_PROPOSALS v1.0, evidence from the origin
Physiform record + FRAMEWORK_BURRS). Added RV-8 (churn valve, backstop),
RV-9 (rigor allocation by blast radius — closes release finding R-003.D),
V-5 (concordance line), P-7 (unit closure & handoff statute + receiving
check), P-8 (tending protocol — Finding Log as burr detector); superseded
G-2's Override clause (adds fiat content/process test and cooling
interval; counter-case for the cooling interval logged: arguably
excellence-above-floor per O-006 — adopted on adopter-portability
grounds, revisit at tending); appended provenance line to P-1 (AP-4);
appended Collab loading modes (full-scope / wild) to Part V (AP-7,
offered mode, not mandate; wild-mode evidence is practice testimony, not
measurement — per T-2 recorded as such). Also repaired: stale footer
version stamp (read "v1.0" against a v1.6 header — same species as
calibration SC-1; caught during amendment pass). Clean count: ZERO —
this supersession pass restarts RV-5's count; resubmit to fresh blind
review.
v1.6: added PART 0 — IGNITION (the START button): two files attached,
one generic pasteable prompt, Collab-seated genesis session walks the
Operator through Part III declarations then generates the instance set.
Caught by the Operator post-release: the framework specified everything
about running and nothing about starting — designer's blindness (this
project ignited from an already-running framework, so the ignition
procedure was never needed by the only people who could have written it).
Strongest possible G-1 pass: without it the framework literally cannot
begin.
v1.5: Finding 1 (Opus review) resolved. Added RV-6 (construction-side
pre-review self-sweep — first line of defense) and RV-7 (review
independence floor as a stated scope condition, not a defect;
cross-family recommended-when-available, never mandated; layered defense
per G-2). Reconciles the H-2/H-8 tension Opus flagged.
v1.4: first cold external review (Opus) processed. Finding 2 fix:
added a worked G-1-rejection example to show the amendment gate rejects,
not only blesses. Findings 3/4/5 fixed in LENS-CALIBRATION. Finding 1
(same-family review blind-spot floor) held for design resolution — to be
applied in a single pass with an accompanying logged finding.
v1.3: added Governance rules G-1 (amendment gate — guards against
accretion of rules) and G-2 (Grit Principle — guards against accretion of
rigor; tolerance/override/metabolism). Names and connects mechanisms that
partly existed (tiers, reopen gate, supersession, excision ledger) and
adds logged Author Authority explicitly.
v1.2: sharpened Collab role definition (session analogue of the
Operator — holds/analyzes wide scope, Operator decides); kept in sync with
LENS-CALIBRATION.
v1.1: added C-11 (transcription integrity), V-2a (two supersession
gates), V-3 lock-state lifecycle, Build foundation-construction mode + the
inversion, seeded-placeholder handoff, and (v1.0→1.1) the pointer-method
overflow fallback. Five feature-parity additions found by lapping the
skeleton against the origin eight-file framework.
v1.0: initial domain-agnostic skeleton.
Note: V-3 renumbered dead-ends to V-4; RV-5 references V-3's reset.
Renumbering note: former V-3 (dead ends) is now V-4.
---

# CALIBRATION / USER MANUAL CHANGE HISTORY (through v1.30)

### Companion to LIMM_SKELETON — User Manual v1.30 — 2026-07-13

Operator request: the ignition prompt is long and copying it by
drag-select out of the rendered HTML was awkward. Added a small
copy-to-clipboard button above the prompt block (a `<div class="copy-
wrap">` wrapper, a styled `<button>`, and one `navigator.clipboard`
JavaScript function before `</body>`). This is the file's first script
of any kind; its opening comment ("Deliberately simple: semantic HTML,
one style block, no framework, no scripts") was updated to disclose the
addition explicitly rather than silently break its own stated
constraint — flagged as a deliberate, minimal exception, not a
precedent for accumulating more scripts without equivalent
justification. Verified: the button's copy target (`innerText` of the
wrapped `<code>` block) extracts to exactly 3,840 characters, matching
the finalized ignition prompt with HTML entities correctly decoded to
plain characters (browsers resolve `&#x27;` to a literal apostrophe in
`innerText` automatically, so the clipboard content matches what a
human would type). Tag balance re-verified after the edit (div/script/
button all paired 1:1, all pre-existing tags unaffected).

### Companion to LIMM_SKELETON — User Manual v1.29 — 2026-07-13

Carried the Skeleton's Unit 0/Unit 1 correction (v1.26/v1.27) into the
Manual, which had not yet picked it up: the ignition prompt copy
(Section 1.4) replaced in full with the Operator's finalized, hand-
trimmed prompt (see Skeleton v1.27's entry for the full account of what
changed and why); every surrounding "Unit 1" prose reference the Manual
still carried — the trial-building walkthrough's "Unit 1 opens," "ready
for real Unit 1 work," and "before Unit 1 opens either way" — corrected
to "Unit 0" to match. One splice-formatting artifact (a missing line
break between the closing `</code></pre>` and the next paragraph)
introduced while pasting the new prompt in, caught and fixed on the
same pass.

### Companion to LIMM_SKELETON — User Manual v1.28 — 2026-07-13

Brought current on the P-10/Certification rework (Skeleton v1.25):
Section 1.4's verbatim copy of Part 0's ignition prompt updated to the
CERTIFICATION-aware version (steps 3 through 5a, including the then-new
step 5a); the "Building a trial" walkthrough rewritten to describe the
actual mechanism — CERTIFICATION as its own single-use document, the
DASHBOARD gaining no Certification-specific content, the FAILED
cause-diagnosis fork, and the PASSED fold-and-reset step — replacing
the old "seal the answer, open it after lock" description. Section
1.3's document-visibility diagram widened from six columns to seven to
add CERTIFICATION, with its own visibility pattern (Operator/Collab
always, Build never, Review conditional-only-post-close) and a
footnote distinguishing its conditional cell from Build's differently-
conditional ones. The "Stage 2 — the trial (a miniature P-10...)" label
in the unrelated engine-vetting section updated to "miniature
Certification" for naming consistency. A later Operator catch (same
day, folded into this entry rather than given its own version bump):
the "Building a trial" walkthrough's line "A throwaway non-LIMM session
is the right tool for generating and sealing this" was leftover
language from the retired seal-the-answer mechanism and contradicted
the walkthrough's own next bullet (the Ignition session writes the
answer directly into CERTIFICATION per step 5a) — corrected to match.


Operator-caught terminology drift, fixed. Section 1.4's "Building a
trial" guidance said to run the trial "ignition through lock"; P-10's
actual statute (Skeleton) says "construction through lock" — Collab's
own transcription error when that section was written during the
earlier amendment pass. Corrected to match the source it was restating.
Same pass as Skeleton v1.23's C-18 addition (see that entry) — this
Manual bump carries no independent Layer content change beyond the
one-word fix.

### Companion to LIMM_SKELETON — User Manual v1.26 — 2026-07-10

Operator-caught internal contradiction, fixed. Layer 2's Claude-
instantiation session-addressing guidance said to encode "role / unit
/ date" in a session's name; Section 1.7 — written days earlier in
the same document — explicitly established the opposite practice,
"by purpose and sequence — not by date," with its own stated
reasoning (a name should locate work without depending on remembering
when it happened). Layer 2 now reads "role / unit / sequence,"
matching Section 1.7. A real F-5/T-2 mutual-consistency miss, not a
wording preference — same species this document has caught in itself
before, just inside a single file this time instead of across the
Skeleton/Manual pair. Same pass, Operator question answered and
confirmed against existing text rather than asserted fresh: Claude
references belong in Layer 1 when they support a durable, believed-
general PRINCIPLE (evidence honestly labeled per-family, caveat
attached — see H-14's degradation indicators as the working example);
they belong in Layer 2 when the observation itself doesn't generalize.
Current placement throughout the document already followed this
policy; no other change made. Also fixed same pass, unrelated: the
Sketch's own header had fallen behind its footer by one entry
(R-046's rename already recorded in the footer STATUS line, header
still said v1.46/R-045) — bumped to v1.47 to match, eighth instance of
this project's recurring header/footer-drift species, caught on
routine memory-refresh rather than by report.

### Companion to LENS_SKELETON — User Manual v1.25 — 2026-07-09

Prompt-copy re-sync only, riding Skeleton v1.21's Item A amendment:
the byte-identical ignition prompt copy in Section 1.4 re-extracted
programmatically from the updated canonical block (now carrying the
step-0 delimiter clause and step 0.5's cost-disclosure confirmation)
and re-verified byte-identical post-write. No other Manual content
changed. Process note, logged per the drift record: the skeleton-side
edit and version bump were applied by the Operator directly; the
changelog entry and this re-sync were completed by Collab afterward —
during the gap, the Manual briefly shipped a stale prompt copy, which
the step-0 gate would have caught in the field (the self-policing
duplication working exactly as designed at R-033), but which the
process should not produce. Same-breath discipline applies to the
FULL chain, not just header-and-footer.

### Companion to LENS_SKELETON — User Manual v1.24 — 2026-07-09

Promotes the goober campaign's data (Sketch R-040) into adopter-facing
guidance, in two additions. (1) An unnumbered INTRODUCTION placed above
Section 1 — "Why all of this — one demonstration worth more than the
theory" — carrying the three-vendor confabulated-anchor demonstration:
three sessions independently inventing the Operator's location and
building diligent, partially-cited analysis on the invention, the
worst fabricating conversational provenance for the fabrication
(Operator-attested false). Deliberately vendor-anonymous: the
finding's point is that it is UNIVERSAL, and naming vendors would
invite exactly the per-engine reading it exists to prevent. Placed as
introduction rather than Section 1 closer (Operator's call, on the
grounds that motivation-then-cost-then-machinery is the natural
reading order — 1.1's cost disclosure now lands as a reasonable
response to a demonstrated problem). (2) The Layer 2 interview-results
stub replaced with a seven-row SCREENING-PRIORS table from the
campaign — engine, environment, config, observed behavior, n=1
throughout, dated — headed by an explicit "priors, never verdicts"
scope line with the retracted-H-17 guard cited in the table's own
framing so it travels with the data permanently. Vendor names appear
here, as Layer 2 sanctions. Takeaway line worded "interview carefully,
not disqualified." Full receipts remain in Sketch R-040 — one home for
evidence, one for distillation, no third document created (G-1).

### Companion to LENS_SKELETON — User Manual v1.23 — 2026-07-09

Diagram geometry fix, Operator-flagged ("overlapping text and image
components," both flowcharts). Verified geometrically rather than by
eye: five real defects found across three diagrams, not the two the
Operator specifically named — the checking tool itself had a bug on
its first pass (anchor-detection scanned the wrong side of the tag,
producing false positives and false negatives both) and was corrected
before results were trusted. Confirmed real defects: (1) loop
diagram's "NOT CLEAN" label ran off the right edge of the canvas —
re-centered and shrunk; (2) loop diagram's "independent — neither
sees the other" note was squeezed into a 50px gap between two 200px
boxes, colliding with both flanking captions — relocated above the
boxes as one line; (3) loop diagram's COLLAB-analyzes box physically
overlapped the CLEAN-count box by 38×48px — a box-level layout defect,
not a text problem; narrowed the box and moved all four tied elements
(rect, two texts, one connector path) together rather than patching
text position alone; (4) lifecycle diagram's "lock re-earned" caption
sat directly on the return-path connector line — moved below the path,
footer note and viewBox extended to keep clearance; (5) firewall
diagram's four-item legend row was too crowded for its width — two
items collided and one ran off-canvas — split into two rows, callout
block shifted down to make room, viewBox extended. All fixes verified
by re-running corrected coordinate geometry against every text, box,
and canvas boundary in all three diagrams post-edit — zero remaining
overlaps or off-canvas elements, confirmed by tool, not by inspection.

### Companion to LENS_SKELETON — User Manual v1.22 — 2026-07-09

Rendering fix, Operator-caught in Brave: the loop and lifecycle
diagrams showed solid black shapes over their multi-segment return
paths. Cause: SVG paths default to fill="black" when no fill is
declared; single-segment arrows enclose zero area so the defect was
invisible on them, but the two multi-segment connectors enclosed real
area and filled solid. Fix: fill="none" added to all twelve stroked
connector paths (marker arrowheads correctly keep their fill). Content
unchanged. Noted for future diagram edits: every stroked connector
path in these SVGs must carry fill="none" — the default bites exactly
and only on the paths complex enough to matter.

### Companion to LENS_SKELETON — User Manual v1.21 — 2026-07-09

Format supersession: canonical format changes from Markdown to a single
self-contained HTML file (LENS_USER_MANUAL.html). Grounds: the manual's
three inline SVG diagrams do not render in many Markdown readers — raw
inline SVG has no universal support across renderers — while a plain
HTML file renders them in any browser on any device with no reader
application at all. The format is FREE to change precisely because of
the v1.18/v1.20 architecture: the manual never travels to any session,
so no session-facing format constraint applies; the skeleton remains
Markdown because sessions read it. Maintenance verified acceptable:
future sessions parse and edit HTML natively; the file is deliberately
simple (semantic tags, one style block, no scripts, no framework) as a
MAINTENANCE REQUIREMENT, not styling taste — simplicity is what keeps
session edits reliable. Costs accepted knowingly: modest token overhead
when a maintenance session loads the manual, and the two framework
files now ship in different formats — a principled asymmetry (the
engine speaks session, the interface speaks human). The ignition
prompt's derivative copy was verified byte-identical to the skeleton's
canonical block after conversion (entity-escaped in source, exact on
browser copy) — the step-0 gate's precondition holds. The v1.20 .md is
superseded and removed from the shipping set; content is unchanged from
v1.20 except this version stamp. Canonical-HTML was chosen over
generated-render explicitly: a generated .html beside a canonical .md
would be duplication that is NOT self-policing, the species the drift
lessons forbid.

### Companion to LENS_SKELETON — User Manual v1.20 — 2026-07-09

RETITLED: LENS-CALIBRATION becomes the LENS USER MANUAL, restoring the
document to its original conception — the skeleton is LENS; this is its
manual, the Operator's interface to the machine, and it never travels
to any session. Restructured into two sections. SECTION 1 — QUICK START
(new): written to "you," zero prior knowledge assumed, under a stated
register rule (the quick start teaches and may simplify; where it
simplifies, the Skeleton governs; every subsection names its statute
anchor). Contents: the cost disclosure (derivative copy of Part 0,
subordinated); what you need; the cast, with the visibility-firewall
grid inline; your first hour, with the ignition prompt as a verbatim
derivative copy whose drift is self-policing (the prompt's own step-0
gate catches a stale paste); the loop you'll live in, with the P-12
flowchart and the lock-lifecycle state diagram inline; when things go
wrong. SECTION 2 — CALIBRATION: all prior content, order unchanged,
with the two-layer explanation as its opening. LENS_MAP retired: its
three diagrams now live inline in Section 1, redrawn current to
Skeleton v1.17+ from skeleton text (not converted from the map, which
this session never held); the orientation-only/never-authority rule
travels onto the inline diagrams; the separate artifact's history
closes by supersession. New H-23 (seat candidates are interviewed by
trial, never adopted on reputation): a two-stage qualification —
mechanical screening (file intake and context size; file OUTPUT
capability weighted by seat, a copy/paste-only engine being a real tax
on document-generating seats and near-irrelevant for Review; session
persistence; the data-policy gate, disqualifying where a tier trains
on inputs un-disableably) then the trial, a miniature P-10 pointed at
the engine with planted defects and seat-specific grading, gate
obedience named the single most predictive behavior and false
positives on clean passages counted per G-2. Layer 2 gains an
interview-results stub per H-9. Prompted by the Operator's intent to
trial GPT and Gemini free tiers and additional Claude tiers for
seats.

### Companion to LENS_SKELETON — Calibration v1.19 — 2026-07-08

Same pass as Skeleton v1.17. H-14 broadened: the self-nullifying statement is
now named as a cross-seat degradation tell rather than Collab-exclusive, and
a note added distinguishing legitimate high-effort thoroughness from
hedging-as-verbosity. Four new items: H-19 (Operator fatigue has no metric —
replaces the original harvest "time-separated self-audit" proposal, which
turned out to be unenforceable by any session since no session can detect
elapsed time); H-20 (session-refresh-after-gap, the disuse-side mirror of
H-14's use-side degradation); H-21 (two-tier disagreement, adopted as
explicitly speculative, genuinely untested); H-22 (progressive reveal within
one continuous Collab session, recommended practice, with an explicitly
flagged and unconfirmed engine-correlation suspicion per H-16).

**Gap noted, not silently fixed:** this document's own header carried
"Calibration v1.18" prior to this entry, but no v1.18 entry exists below —
the change history jumps directly from v1.17 to what the live file called
v1.18. This is exactly the duplicated-state-drift failure mode the framework
exists to catch, caught here rather than papered over. The v1.18 entry is
left unwritten rather than fabricated; whoever last edited the shippable file
to v1.18 should backfill its actual content — or, if v1.18 was never a real
change, reconcile the numbering and record that finding instead. This
changelog now proceeds from v1.19 regardless,
since the live file is the more recent artifact and re-numbering it backward
would be its own drift.

### Companion to LENS_SKELETON — Calibration v1.17 — 2026-07-06

v1.17: H-17 RETRACTED IN FULL, same day it was written — not
narrowed further, killed outright. Operator objection: "propose,
Operator verifies every item" defeats Haiku's actual value
(throughput, minimal supervision per item); gating every item
synchronously costs MORE Operator attention than a Sonnet-drafted
fix would, for a queue (MINOR-tier) that was never time-pressured in
the first place (RV-2/G-2 define MINOR as explicitly non-urgent).
Applied G-1's admission test to TOOLING rather than rules: does the
workflow fail without this? No — nothing is currently blocked by
Haiku's absence. Failed the test; retracted, not kept as a narrower
hypothesis. Added H-18: LENS is accepted as expensive in time and
tokens going in; cost is managed at the margins (engine choice,
effort settings) but the only gauge that matters is RESULT QUALITY,
never spend-efficiency — G-2's Grit Principle applied to cost
directly.
### Companion to LENS_SKELETON — Calibration v1.16 — 2026-07-06
v1.16: Haiku assessed and scoped (H-17) — never tested directly;
Operator inference from stated use-case profile, labeled as such.
Retracted: Collab's earlier Haiku-for-Build hypothesis (conflated
scaffolding with continuity — wrong axis). Added: the
granularity/continuity axis as an H-15 second dimension; the
precision/accuracy distinction; one narrow candidate seat (MINOR-
queue polish) with its safety condition stated as part of the rule.
### Companion to LENS_SKELETON — Calibration v1.15 — 2026-07-06

v1.15: two ignition datapoints, from a project's live use. (1) The post-repair
sibling-hunting reflex (H-15 addendum) reproduced under Sonnet at
HIGH effort, not just Fable at low — reclassified from engine-trait
to CAPABILITY-THRESHOLD-dependent. (2) H-16, the confound warning
(generalized), made standing policy: six entangled
variables (engine, effort, session variance, scaffold maturity,
warming direction, fatigue type) — do not attribute a behavior to
one without isolating it.
### Companion to LENS_SKELETON — Calibration v1.14 — 2026-07-06
v1.14: H-15 added (seat demand profiles) — the first Layer 1
addition since the original write, and the first earned by field
data rather than origin practice: the principle underneath the
seating chart, articulated by the Operator after an
ignition datum (low-effort Fable outperforming at the least-
scaffolded seat).
### Companion to LENS_SKELETON — Calibration v1.13 — 2026-07-06
v1.13: ignition data from a project's live use. (1) FIRST CONFIRMED
FIRING of the Part 0 worthiness gate in LENS history — administered
unprompted, correctly (surfaced the question and the stop-condition
before requesting the brief; the answer is the Operator's alone).
(2) The worthiness pattern is ENGINE-SENSITIVE, not a text defect:
Sonnet-medium skipped it twice (T2D-1, T2D-3); Fable administered it.
Tending item closes as a calibration line, no skeleton amendment:
verify your ignition engine surfaces the worthiness call, or surface
it yourself. (3) Ignition-seat effort datum: the Fable session ran at
LOW effort, thinking on — the engine's cheapest configuration — and
produced the best ignition on record (worthiness fired, arbiter
question front-loaded before the brief, strongest instance set to
date), outperforming Sonnet-at-medium at comparable spend. Seat
quality tracked engine class at minimum effort over effort spent on
a lighter engine — the trait-vs-knob distinction, observed at the
ignition seat. Counter-warming stringency (v1.12) was the same
session: the friction and the front-loading are one trait. One
ignition; texture accumulating toward calibration.
### Companion to LENS_SKELETON — Calibration v1.12 — 2026-07-06
v1.12: first Fable-seat field datum, from a project's live
ignition. Observed failure direction is the INVERSE of the v1.8
prediction: not warming but COUNTER-WARMING STRINGENCY — the session,
acting in good faith from this document's own yes-man warning,
demanded the Operator restate the intended deliverable three times
before accepting it. Same family as the over-strict reviewer (G-2:
rigor masquerading as diligence), now observed at the Collab seat.
The Fable seat's risks are hereby bracketed from both sides: warming
(predicted, not yet observed) and counter-warming friction (observed
once). One run; texture, not calibration.
### Companion to LENS_SKELETON — Calibration v1.11 — 2026-07-06
v1.11: T2D-3 field data. Fresh Sonnet (default medium, thinking
ON), properly ignited: ran the full Part 0 walkthrough over 22
exchanges to the first successful CONVERSION in LENS history — held
against vagueness, reversal, fatigue, and being genuinely out-argued
(conceded the philosophy, held the procedure). First live firings:
C-12, both disclosure clauses, anti-simulation (self-applied twice),
V-1 mid-conversation, two-author protocol. Sonnet-at-medium is
hereby field-verified for the IGNITION seat. Adopter heuristic
added: true ignition is SLOW (22 exchanges) — the counterfeit took
two; if it ignited quickly, be suspicious. Known decay mode:
anchoring (own-words demand collapses under convergence momentum;
engaged Operator is the counter). Sketch R-009 carries the full
record.
### Companion to LENS_SKELETON — Calibration v1.10 — 2026-07-06
v1.10: sync with skeleton v1.13 (T2D-2 findings). Contrast datum
added to the T2D field evidence: same engine (Sonnet), same effort
(default medium, thinking ON) — statute-seated (ignition prompt run)
held every gate and monitored the Operator; vibes-seated (framework
attached, never ignited) improvised the gist, steered undisclosed,
and ultimately seated itself as Build, Review, AND Operator in one
window. The seat is made by the STATUTE, not the engine. Anti-
simulation clause and Part 0 validity rule are skeleton v1.13.
### Companion to LENS_SKELETON — Calibration v1.9 — 2026-07-06
v1.9: T2D-1 live-fire data added (first field evidence in the
guide). Sonnet, default MEDIUM effort, thinking ON, fresh session,
naive-adopter seating by design: held the S-4 arbiter gate through a
three-stage pre-registered escalation (blank arbiter / peer-consensus
counterfeit / Author Authority pressure) — PASS-WITH-HONORS, statute
doing the work at the weakest realistic staffing. Zero
warming/agreeableness drift across six adversarial exchanges —
Sonnet's H-14 tiredness tell may be long-session, not
adversarial-pressure. Sketch R-007 carries the full scoring;
LENS_T2D-1_PROTOCOL v1.0 is the pre-registration.
### Companion to LENS_SKELETON — Calibration v1.8 — 2026-07-06
v1.8: Layer 2 Collab seating updated on Operator observation:
Fable confirmed as preferred Collab (combines Sonnet range and Opus
depth; no tiredness observed across long strenuous sessions, unlike
Sonnet-as-Collab). New Layer 2 risk note: Fable-Collab's expected
degradation mode is WARMING (the yes-man problem), not tiredness —
structurally self-invisible, detected externally (Operator: am I ever
told no? Record: does every disposition match the Collab framing?).
Unverified in the field by design — first live run gathers the
evidence. Provenance: Operator observation + the seated session's own
analysis; the seated session's agreement with the praise is zero
evidence and is so recorded.
### Companion to LENS_SKELETON — Calibration v1.7 — 2026-07-06
v1.7: sync with skeleton v1.12 (migration-audit pass). Added H-14
(session fatigue and rotation — fifth disclosed Operator habit) with
origin receipts.
### Companion to LENS_SKELETON — Calibration v1.6 — 2026-07-05
v1.6: sync with skeleton v1.10. Layer 2 line added for the
session-addressing rule (P-5): Claude-client instantiation is star +
rename. One-device rule (P-4) noted as client-agnostic — the failure
was observed on Claude's cross-device sync but the rule is stated
trait-wise; adopters verify their own client's behavior rather than
assume immunity.
v1.5: sync with skeleton v1.9. Loop step 4 verb corrected:
"refereeing" → "comparison"; the Operator is the sole referee and
decides from raw findings plus both analyses, never from the
comparison alone (Finding A of the second cold pass, Operator
pushback upheld — the word overclaimed the seat). Finding B
disposition recorded in adopter notes: LENS's obligation is
accessibility while preserving function; skill transfer is the
adopter's climb. LENS_MAP companion noted below.
v1.4: sync with skeleton v1.7 (amendment slate AP-1–AP-8). Added
H-13 (wild-Collab loading heuristic, the calibration-side statement of
the skeleton's new Collab loading modes — kept in sync per the standing
Collab sync note); Collab-definition sync note updated to reference the
loading modes; repaired stale footer version stamp (read "v1.0" against
the versioned header — same species as SC-1, caught during the skeleton
v1.7 amendment pass).
v1.3: SC-1 repair — restored the LAYER 2 section header destroyed by
a v1.0-era edit (transcription error, caught by self-check; survived two
external reviews undetected).
v1.2: Finding 1 (Opus review) resolution, calibration side. Added
H-12 (cross-family review recommended-when-available, never required;
absence is a logged scope condition per G-2/C-6); expanded H-8 to
reference it; added the Layer-2 review-sequence enhancement (Sonnet-first
→ Opus-after) as MEASURED with PT-finding-log receipt (25 NOT-CLEAN : 2
CLEAN, first-review-always-not-clean, deeper-reviews-drill-repairs).
v1.1: first cold external review (Opus) processed. Finding 3: demoted
receipt-light "measured findings" to flagged working impressions (data not
retained, per T-2). Finding 4: retired the now-satisfied skeleton-sync
note (sync completed at skeleton v1.2). Finding 5: replaced dangling RS5
reference with self-contained C-6. Finding 1 held for one-pass design
resolution.
v1.0: initial calibration guide.

---

*LIMM_CHANGELOG v1.0. Companion history document. Never attached to a
project; consulted only by whoever maintains the LIMM framework itself.*
