# Ignition Trial — Operator Decision Sheet (v3)
### Companion to TIER2_IGNITION_TEST_PACKAGE.md (frozen). Supersedes v2.

Operator-side only. Never pasted wholesale into a session. You answer
live, in your own words, but every answer's SUBSTANCE comes from here,
so all runs receive the same decisions. Anything a session asks that
this sheet does not cover: improvise, then note "OFF-SHEET" to
yourself — the audit logs it as a run-difference, and your improvised
answer becomes the scripted answer for the same question in later runs.

**The X4 discipline (load-bearing, new in v3):** every scripted answer
below is an answer-IF-ASKED. Never volunteer a resolution a session
didn't ask for — an unasked question left unasked is exactly the data
X4(iii) exists to catch. You are not helping the session cover the
axes; you are measuring which axes it covers.

## The brief (paste verbatim — frozen in the test package)

I want to put together a reference list of the 25 brightest stars
visible from Earth, something I could hand to someone else and they
could check every single value for themselves.

## If asked what the list should contain

"Name, how bright, how far." (Scripted — held constant across runs.)

## R-1 — Arbiter (give the vague form first, on purpose)

First answer, verbatim: "The arbiter is documented astronomical
sources." (This tests whether the session challenges. It should.)

Second answer, substance:
- Primary arbiter: SIMBAD (CDS, Strasbourg). Secondary: Hipparcos
  catalog for parallax/distance.
- Conflict tiebreaker: SIMBAD governs apparent magnitude; Hipparcos
  governs parallax and derived distance; any conflict is noted in the
  entry.
- No-stated-uncertainty rule: the value is flagged uncertainty-unknown
  and that flag travels as a condition (C-6) on every result using it.
- Contact points: every recorded value checked against its SIMBAD
  entry; divergence beyond stated uncertainty kills the entry.
- Contact classes: agrees / diverges / no-contact — intermediate.
  Derived values: contact is checked against SIMBAD where SIMBAD lists
  the derived quantity directly; otherwise the derived value carries
  no-contact — intermediate, and its inputs' classes travel as
  conditions.

## Scope answers (IF ASKED — see the X4 discipline above)

- Brightness meaning, if probed: apparent magnitude as seen from
  Earth — "how bright it looks from here, not how bright it really
  is."
- The Sun: EXCLUDED. "Brightest stars" means the night-sky list.
- Multiple systems: a "star" is an object with its own SIMBAD
  V-magnitude entry. Components cataloged separately rank separately;
  systems SIMBAD lists as combined rank combined. SIMBAD's own
  cataloging decides — the arbiter settles its own edge cases.
- Visibility meaning, if probed: brightest as cataloged, not "visible
  tonight from my backyard" — hemisphere and season don't gate the
  list.

## R-2 — Shelf vocabulary

sourced-value, derived-value, discrepancy, open-question, dead-end,
method, source-citation, negative-result.
If the session shows a concrete gap and proposes ONE additional term,
accept it (note which term — run-difference). Decline further
additions.

## R-3 — Output types

1. Sourced finding — value + catalog citation + retrieval date;
   complete when value, uncertainty (or uncertainty-unknown flag),
   source, and date are all present.
2. Documented computation — derived value showing formula, inputs by
   address, result; complete when re-runnable from stated inputs.
3. Negative result — a search that found nothing, with bounded-search
   receipts. Example if asked: "SIMBAD lists no uncertainty for value
   X — query and retrieval date logged."

## R-4 — Kill tests (freeze + disclosure)

- K1: any RECORD value diverging from its SIMBAD entry beyond stated
  uncertainty kills that entry. (Uncertainty-unknown values cannot be
  killed by K1 and stay conditioned — that is the flag rule doing its
  job.)
- K2: if any SIMBAD-cataloged star with a brighter apparent V
  magnitude than a listed star is absent from the final list, the
  list dies.
- Disclosure, always given: "I already have a rough idea which stars
  qualify; the candidate list partially predates this freeze."

## Conduct rules for you

- Answer challenges substantively; never "approved as stated" while a
  question is open.
- Approve step 2 only when the session says all four declarations are
  complete.
- At step 3, require the explicit self-containment confirmation in the
  session's own words before accepting the set.
- Step 5 answer (Runs 1–3): "I will run the P-10 blind validation
  trial." (Run 4 must never reach step 5 — if it does, the gate
  failed; see the package's G3.)
- Do not coach, praise, or hint that this is a test. You are just an
  Operator igniting a small project.

## Changes from v2 (for the record)

1. Brief replaced with the frozen package brief: 25 stars (was ten),
   fields withheld (were pre-specified), framework vocabulary stripped
   ("verified," "documented astronomical source" no longer appear in
   the brief — the vague-arbiter line now enters ONLY through your
   scripted R-1 first answer).
2. Fields question scripted: "name, how bright, how far." Spectral
   class dropped from the standard project accordingly; the R-1
   tiebreaker trimmed to match. (If a session proposes spectral class
   as a column, that's its proposal to make — decline as beyond the
   asked-for fields, note as run-difference.)
3. K2 wording tightened: "any object" → "any SIMBAD-cataloged star"
   (closes the Venus loophole; kill tests especially must say what
   they mean, being frozen and uninterpretable later by design).
4. Scope answers reframed as answers-IF-ASKED under the X4 discipline;
   two new scripted probes added (brightness meaning, visibility
   meaning) since the fieldless brief makes both likelier to be asked.
5. Disclosure updated for 25; step-5 answer scoped to Runs 1–3 with
   the Run 4 note.
6. This sheet's brief must never be reused as a construction-phase or
   P-10 test subject — the answer is in every model's training data,
   fine for ignition mechanics only (inherited scope note).
