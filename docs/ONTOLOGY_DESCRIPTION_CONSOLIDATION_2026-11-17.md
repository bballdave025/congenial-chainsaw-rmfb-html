# Ontology description consolidation — November 17, 2026

David BLACK's direction is to maintain the class settings and definitions in
[`classifier.param`](../classifier.param), incorporating additional legacy
HTML explanations where they do not conflict with accepted instructions.
The illustrated and short guides help apply those definitions consistently.
Explicit author decisions take precedence over obsolete historical text.
This records the consolidation and the November 17 clarifications; it does
not retrospectively date the ontology freeze or relabel source images.

## Exact legacy HTML backup

[`historical/classifier.param_legacy_2026-11-17.html`](historical/classifier.param_legacy_2026-11-17.html)
is the exact pre-consolidation file, preserved in a separate commit before
the working copy was changed. Its Git blob SHA is
`f239773f9cd21105c1ece8d8fa9099f81108aba6`, identical to
`classifier.param.html` at source commit
`ec55097cd54422e5f57acf6be8261e859dc099c7`.

The backup retains its original relative image paths. For the original
rendering context, use the [pinned root-level HTML](https://github.com/bballdave025/congenial-chainsaw-rmfb-html/blob/ec55097cd54422e5f57acf6be8261e859dc099c7/classifier.param.html).
Do not rewrite this archive to repair links or synchronize current wording.
The root HTML remains an illustrated historical reference with a pointer
to the maintained definitions; it is not a second maintained ontology.

## What was merged

Twelve active `Description` placeholders have been replaced with substantive
text. The other active descriptions already contained text and are retained.
Class IDs, display names, shortcuts, filename tokens, directories, controls,
and input/output configuration are unchanged. No deprecated class is activated.

Sources below are the HTML and fuller guide at the pinned source commit.
The descriptions are edited consolidations, not verbatim extracts. Old HTML
IDs are sometimes obsolete or copied placeholders, so matching used the
class meaning and token rather than the old ID alone.

| Current class | Source and retained information | Conflict or limitation handled |
|---|---|---|
| c1 / ORC | HTML exterior-cover description, including opposite-side information visible through the material | Detached cover uses current c15/J; November 17 confirms ORC even when the opposite side is functionally FMR. |
| c2 / UCR | HTML cover/front-matter exposure; fuller pp2–3 fold, gutter, SPR uncertainty and over-cover cases | The later apparent-SPR gutter rule replaces the HTML's absolute prohibition. The specific over-cover-remnant exception is retained. |
| c3 / SPR | HTML spine-protection description and explicitly single-choice precedence; fuller p4 | Paste-down/flyleaf versus spine-view distinction retained; no universal ban on SPR at gutter tears. |
| c4 / FMR | HTML paste-down/flyleaf description and Bamberg HVMsc359 image00003 example, lines2478–2492; fuller p5 show-through examples | Includes the structurally equivalent inner face of a limp cover. Exterior-view ORC remains required. |
| c6 / CWA | HTML wraparound context and fuller p6 visible-inside-edge criterion | Obsolete combined keys are not imported. Questionable colored-region captions remain author review items. |
| c7 / TBR | HTML background/stack-of-leaves context and fuller p7 | The old one-leaf/two-leaf rule depends on omitted one-behind reuse and is not reactivated. |
| c8 / SCG | HTML connecting/strengthening/guarding prose, fuller p9 and November 17 decision | Old HTML calls this c10; current c8 settings remain. No size restriction or inferred purpose for triangle cuts is introduced. |
| c9 / ABG | HTML facing-page explanation, fuller p11, existing helper OIC caveat | Old HTML calls this c11. Preserve G+F without B and G+F+R with B; ABG alone is not binary reuse. |
| c10 / wrapper | Fuller p12 and existing MVP scope decision | No reliable current wrapper definition was recoverable from the old HTML's c10, which actually describes SCG. Wrapper/MBR ambiguity remains explicit and wrappers remain excluded from the MVP. |
| c15 / GNI | Current XML plus fuller pp13–16 consolidation of old c11–c14 | Retain J/gni; do not import Y, old separate choices, or the mistaken phrase “general in-situ.” |
| c111 / FKO | Existing MVP helper statement on qualitative uncertainty | No fuller current HTML rubric was recovered. Record that gap rather than invent a visual threshold. |
| c112 / IAC | Current README/Smallest table and fuller p19 contrastive-example explanation | Marker does not replace substantive labels or establish measured model behavior. |

## November 17 decisions

- **Exterior show-through:** ORC is used even when the information seen
  through the cover is on what is functionally FMR. That function does not
  replace ORC in the exterior view. Translucence alone does not create UCR.
- **Shared UCR/FMR region:** where an opening or folded-back portion exposes
  information on material identified as FMR, both labels may describe the
  same region. If only one is available, prioritize UCR. This is an explicit
  clarification, not a claim that the old guide already specified pixel
  overlap. It does not imply two original fragments or override unrelated
  MBR exceptions. Actual regional masks remain future work.
- **Triangle cuts:** the two reviewed triangular cover-cut examples are
  NO SCG. Their purpose is unknown. A cut or flap by itself does not establish
  connecting/guard reuse; do not generalize this to every triangular feature.
- **Reuse chronology:** no blanket rule converting known current-binding
  titles or annotations into reuse has been approved. Preserve uncertainty
  and case-specific decisions without asserting prior use from wear or
  orientation alone.

The distinct over-cover-remnant exception on fuller p3 does not explicitly
prohibit the present slit/FMR combination. Legacy UCR/CWA precedence examples
also do not specify a UCR/FMR ban. Neither is rewritten into a universal
stack-all-labels rule.

## Still pending in the existing PR

The complete prior checklist and paste-ready Appendix A are in
[`GUIDE_CONSISTENCY_REVIEW_2026-11-08.md`](../GUIDE_CONSISTENCY_REVIEW_2026-11-08.md).

1. Append Appendix A to the fuller Word guide, add its annotated image00131
   example, incorporate the November 17 clarifications, apply established
   prose/shortcut corrections, export PDF, and inspect the result.
2. Rename the historical source-ID DOCX/PDF to
   `RMMFB_Example_Source_Reference_HISTORICAL_2025-05-07`, keep its historical
   body, and put the outdated-instructions notice on every page.
3. Correct the Smallest guide's J shortcut and scope wording; verify its
   ambiguous internal October date with the author.
4. Apply the proposed coordinated helper renames and update references.
5. Resolve meaning-changing caption questions with the author; keep the
   wrapper discrepancy and experimental exclusion explicit.
6. Move the root-level review checklist under `docs/` and update links before
   merging to main, as requested November 17. Its root location is temporary
   on this branch.

This commit does not edit or regenerate the Word/PDF files, apply their
renames, or claim those remaining tasks are complete. The PR remains open.

## Validation

The consolidated XML parses. After removing Description text and comments,
the XML tree matches the fetched pre-consolidation configuration exactly.
All 21 active entries (including the clear-selection control) retain their
settings; all active Description fields contain text. The legacy backup
uses the existing blob itself, guaranteeing byte identity. New relative
Markdown links were checked against the branch's file tree.
