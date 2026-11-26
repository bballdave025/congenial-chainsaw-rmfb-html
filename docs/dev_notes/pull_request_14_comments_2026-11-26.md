# Pull request #14: descriptions, comments, and closeout checklist

Archived **2026-11-26 (America/Denver)** from [PR #14](https://github.com/bballdave025/congenial-chainsaw-rmfb-html/pull/14), **Consolidate ontology descriptions and reconcile classification guides**.

This file combines the discussion into a current checklist and preserves the captured PR description and all four discussion comments below. It is a snapshot of the description available at capture time, not a reconstruction of every edit to that description. Source links and original wording are retained so that the reasoning remains reviewable after merge.

Document review baseline: `3a7e9059e9385ea03e8d88d21ea4e46a727073c4`. The later closeout commits add documentation only. PR branch: `docs/binding-context-conventions-2026-11-08`; target: `main`. The PR was open and unmerged when the discussion was captured.

## Current disposition

Dave chose to close the nearly completed ontology PR and defer the remaining editorial and source-search work. The old “Still required before merge” lists below are historical status reports, not a renewed requirement to complete that work. Use the [outstanding-issues checklist](../FIXME_TODO_outstanding_ontology_issues.md) for the current disposition and page-specific details.

## What this PR contains

- [x] Consolidate twelve active description placeholders in `classifier.param` using non-conflicting legacy HTML and guide explanations; preserve class IDs, shortcuts, tokens, directories, and other configuration.
- [x] Preserve the exact pre-consolidation HTML at `docs/historical/classifier.param_legacy_2026-11-17.html`, with source mapping and excluded/obsolete passages documented.
- [x] Explain binding context and visibility: ORC still applies to exterior show-through when the opposite side is functionally FMR; translucence alone does not create UCR. UCR/FMR may share an identified exposed region, with UCR preferred for a single regional label.
- [x] Record the NO SCG decision for the two reviewed triangle-cut examples without asserting their physical purpose or changing the SCG token.
- [x] Preserve the specific MBR exceptions, including uncertain UCR/SPR alternatives for one piece and the ABG distinction; do not count tags as independent source fragments.
- [x] Retain provenance for the reviewed baseline and the still-unrecovered original ontology freeze date/SHA. The November explanation/clarification dates do not establish that original freeze.
- [x] Reconcile Markdown reference tables with the current configuration, distinguish historical proposals from active entries, and rename the helpers descriptively.
- [x] Export the fuller guide with Appendix A and original/cropped/annotated image00131 illustrations; retain its accepted `fko, mbr, orc, ucr, spr` audit annotation.
- [x] Add the November 25 wrapper publication-scope note while retaining c10 in the annotation ontology.
- [x] Rename the historical source-reference DOCX/PDF and add an opening warning plus historical-reference footer on every PDF page.
- [x] Correct the Smallest guide's J shortcut and internal October 3 date, and apply many of the fuller guide's proofreading corrections.
- [x] Preserve the reported Utrecht derivative-quality issue and supplied example with explicit uncertainty about the conversion command and batch extent.
- [x] Record the unresolved items for later work rather than silently treating every caption or source as verified.

## Deferred documentation checklist

- [ ] Correct the residual U-for-UCR captions, GNI drafting residue, and meaning-sensitive captions using current definitions; preserve historical material as historical.
- [ ] Fix Appendix source-ID/figure-number typos and remaining punctuation/grammar.
- [ ] Continue historical example-source verification and later expert wrapper review, without making all source hunting a prerequisite for a first model result.
- [ ] Move the old root consistency review under `docs/`, repair links, and refresh stale pending-work prose and the repository About description.
- [ ] **PR #15 first item:** create `docs/dev_notes/guide_and_ideas_for_pr_15_2026-11-26.md` on the follow-up branch. Collect the bounded OIC-description synchronization task and relevant deferred work there. This file/branch has not been created by this closeout.
- [ ] For that OIC task, compare README descriptions with the extended Markdown helper and the maintained guides. Stitching descriptions already occur in the Smallest DOCX/PDF (PDF p5) and fuller PDF (p18). Add missing explanations or an explicit source link in the extended helper while preserving the distinction between historical IDs and the newer c50–c62 list. Do not activate future model classes by implication.

For plain-text context searches, `rg -C2 twine README.md` shows two lines before and after each match. Ripgrep does not extract text from DOCX/PDF files, so a plain repository search cannot establish that their displayed text lacks a phrase.

## Experiment handoff, separate from documentation completion

- [ ] Record the later, explicit author decision to exclude `No_For_Binding_Reuse/FamilySearch_-_DGS004518368_00660_nbr.jpg` in the derived experimental selection. Preserve the historical original. Fuller p13 supersedes the earlier advice in comment 6725063784 not to exclude it merely for sharing a DGS; this is a precautionary selection decision, not a verified wrapper classification.
- [ ] Apply wrapper-image exclusion and omit the wrapper output/scoring, including its contribution to aggregate metrics. A `_wpr` token does not imply a negative label for another class.
- [ ] Preserve scoped duplicate/provenance decisions and related-view grouping in the derived split; pin the actual merged ontology revision with the experiment.
- [ ] Verify implementation in manifests/model configuration. This PR's documentation does not establish that a split, training job, or Guided GradCAM result exists.

## How to read historical statements below

The November 8 “append to all three guides” proposal was superseded by the later arrangement: Appendix A in the fuller guide, historical warning in the source-reference guide, consistency corrections in Smallest. Word/PDF exports and helper renames have since been completed, with specific residual issues parked.

The November 8 XML change was comments-only; the November 17 consolidation subsequently changed description text. Neither statement implies that every stage of the PR was comments-only. Likewise, **20 non-clear classification entries** and **21 entries including the clear-selection control** describe the same configuration, not conflicting model-output counts.

The old document lengths were 20/18/8 pages; the reviewed fuller/historical/Smallest exports are now 23/19/8. Prior validation statements retain the scope and date of the work they described. The exact legacy HTML backup blob is `f239773f9cd21105c1ece8d8fa9099f81108aba6`.

## Captured source text

The text inside each expandable section is copied from GitHub. Obsolete pending lists remain here as historical records; use the current checklist above for next actions.

<details>
<summary>PR description captured November 26, 2026 — historical pending list retained</summary>

Source: [PR #14 description](https://github.com/bballdave025/congenial-chainsaw-rmfb-html/pull/14).

Several active class descriptions in `classifier.param` pointed to another file, leaving definitions split between the XML, legacy HTML, and shorter guides. This PR consolidates twelve descriptions into the XML while preserving all class IDs, shortcuts, tokens, directories, and other configuration. It records the current rule that ORC still applies to exterior-cover show-through when the opposite side is functionally FMR, and the November 17 clarification permitting UCR/FMR on the same identified exposed region, with UCR precedence in a single-label regional view.

An exact pre-consolidation HTML copy is preserved at `docs/historical/classifier.param_legacy_2026-11-17.html`. The source mapping in `docs/ONTOLOGY_DESCRIPTION_CONSOLIDATION_2026-11-17.md` records which historical descriptions were retained, which obsolete keys or conflicting passages were excluded, and the remaining limits of the documentation. Explicit author decisions govern conflicts; the illustrated and concise guides support consistent application of the maintained definitions.

The PR also supplies the binding-context addendum and an Appendix A draft; reconciles current Markdown helper tables with the XML; distinguishes historical extension proposals from active classes; records wrapper exclusion from the current MVP without deleting its ontology entry; and preserves the reported Utrecht image-processing quality issue with its supplied derivative. The reviewed baseline and unknown original freeze date remain explicit in `ONTOLOGY_PROVENANCE.md`.

**Still required before merge**
- Edit/export the fuller guide, including Appendix A, the annotated image00131 example, accepted clarifications, and established shortcut/prose fixes.
- Rename the historical source-ID DOCX/PDF and add the outdated-instructions notice on every page while preserving its body.
- Correct the Smallest guide and verify its internal date; resolve the remaining meaning-changing captions with the author.
- Apply the coordinated helper renames and update links.
- Move the temporary root review checklist under `docs/` and update links.
- Update the GitHub About description as planned.

**Validation:** the XML parses; all non-description configuration matches the pre-consolidation XML; all 21 active entries retain their settings. New relative Markdown links resolve against the branch tree. No new trailing whitespace was introduced. The HTML backup uses the identical existing Git blob. Earlier helper-table validation remains recorded in the review. Word/PDF binaries, training code, source-image filenames, and dataset manifests have not been changed by this consolidation.

</details>

<details>
<summary>Comment 6724280159 — November 8, 2026 at 9:52:04 AM MST</summary>

Source: [original comment](https://github.com/bballdave025/congenial-chainsaw-rmfb-html/pull/14#issuecomment-6724280159); author: `bballdave025`.

Pre-merge clarification and remaining document work (November 8)

This PR explains a procedure David confirms was locked earlier. November 8 dates the explanation, not a newly adopted ontology rule. Expected model-learning benefits remain a hypothesis for the current MVP study.

**Recorded in commit edd505e5d00dc1e5b864e7b861a06930f7a0ac51**
- Pinned the reviewed pre-addendum baseline: `c8402b403055774d9eb7732952ad13c80d92b83f`.
- Added `ONTOLOGY_PROVENANCE.md`, distinguishing that snapshot from the unrecovered original freeze date/SHA. Selected methods/context/protocol documents in `fhtw-paper-code-prep`, `rib-wrist-in-bin-din`, and `manuscript-waste-reuse-finder`, plus this repository's history, were checked. The vision document's “Frozen (v1)” is explicitly not the definitional project ontology.
- Preserved the guide's exception: UCR and SPR used as alternatives for one uncertain piece do not alone warrant MBR. This is separate from several applicable contexts in regions of one original writing surface.
- Updated the README's introduction and made the documentation-only scope explicit.

**Word/PDF comparison**
David's recollection is supported: the `1pg_each_-_resizes_to_show_MS_IDs` guide contains highlighted source/manuscript identifiers. It is not interchangeable with the fuller guide:
- Source-ID guide: 18 PDF pages; latest DOCX change May 7, 2025, commit `725720cd12269ce04764c535dbafaae92d4be1c8`.
- Fuller guide: 20 PDF pages; latest DOCX change August 16, 2025, commit `a3afe0847a3bd77b6b4a69bdcca76a1492194601`. Its page 3 has a UCR continuation dated July 18, 2025 that the shorter guide lacks.
- Please review the c8 continuation: page 9 of the source-ID guide says keyboard **B**, whereas page 10 of the fuller guide says **C**.
- The older UCR example already describes folded-back portions as UCR, internally dated May 5, 2025. These dates support earlier documented usage; none independently establishes the experimental freeze date.

**Outstanding:** no DOCX/PDF has been appended or regenerated. Preserve source captions, reconcile the c8 wording and other content differences, then append the dated addendum to all three maintained root DOCX guides and export matching PDFs. Historical snippet copies remain historical. The Markdown clarification can be reviewed independently; it does not claim that Word/PDF synchronization is complete.

**Audit clarification:** David has confirmed the erroneous source identifier in the reviewed duplicate pair as a typo after source comparison. Only the exact historical mechanism remains unknown. He has also explicitly approved adding SPR to the accepted ORC/UCR annotation, retaining FKO and MBR. That is an image-label correction under the existing ontology. The detailed case and historical filenames stay in the audit checkpoint; no image files were renamed/deleted by this PR.

**Repository About description:** the README is updated, but GitHub's separate About field is still unchanged. The connected tools cannot edit repository metadata, and the browser is signed out. Suggested replacement:
> RMMFB classification ontology and illustrated annotation guides, maintained in Word with PDF exports, XML classifier configuration, and concise Markdown references.

Validation: XML parses and all non-comment content is unchanged; Markdown links and whitespace checks pass. The PR remains open for David's review; no merge performed.

</details>

<details>
<summary>Comment 6725063784 — November 8, 2026 at 11:01:44 AM MST</summary>

Source: [original comment](https://github.com/bballdave025/congenial-chainsaw-rmfb-html/pull/14#issuecomment-6725063784); author: `bballdave025`.

Updated on branch `docs/binding-context-conventions-2026-11-08` at **70a4f96f64d7ee75575770d4d274da28bdbf448a**.

[Complete consistency review and paste-ready appendix](https://github.com/bballdave025/congenial-chainsaw-rmfb-html/blob/70a4f96f64d7ee75575770d4d274da28bdbf448a/GUIDE_CONSISTENCY_REVIEW_2026-11-08.md).

This supersedes my earlier suggestion to append the explanation to all three Word guides. The plan is:
- Fuller 1-or-2-page guide: in-document **Appendix A**, with `[include annotated image here]`, plus the identified consistency corrections.
- Older source-ID guide: preserve historical body content; rename and add an every-page outdated-instructions footer.
- Smallest guide: consistency corrections only.
- Both Markdown helpers: coordinated descriptive renames proposed for David to apply.

Current keyboard discrepancies follow `classifier.param`, per David: **J for gni**, **R for UCR**. The helper tables now match all 20 active XML entries. The c8 historical B versus current C difference, wrapper/MBR exception, G/MBR exception, older future-phenomena IDs and nbr collision, missing reference rows, and smaller caption issues are documented.

**Wrapper scope decision:** retain c10 in the frozen ontology but exclude wrapper images and its output from this MVP experiment. FamilySearch DGS004518368 images38–40 and the partially unwrapped St. Gallen Cod. Sang. 692 example explain the caption conflict. None of those named examples was found in the audit-matching 3331 inventory; it has zero wpr tokens and zero Wrapper_Reuse paths. The unrelated same-DGS image00660 is not grounds for exclusion. This does not prove absence of visually unrecognized wrappers.

**Still for David before merge:** DOCX/PDF edits and exports, historical-source footer/rename, helper renames/link updates, and repository About description. No Word/PDF files have been edited by me. No image deletion or derived manifest/model-head implementation has occurred. The EG002 accepted source and tag set remain DGS008279842_00131 with fko, mbr, orc, ucr, spr.

</details>

<details>
<summary>Comment 6725332096 — November 8, 2026 at 11:26:06 AM MST</summary>

Source: [original comment](https://github.com/bballdave025/congenial-chainsaw-rmfb-html/pull/14#issuecomment-6725332096); author: `bballdave025`.

Added the requested [important quality explanation](https://github.com/bballdave025/congenial-chainsaw-rmfb-html/blob/ec55097cd54422e5f57acf6be8261e859dc099c7/docs/dev_notes/FIXME_TODO_important_quality_explanation.md) in commit `ec55097cd54422e5f57acf6be8261e859dc099c7`.

It records the exact filename `UnivUtrecht_-_F-oct-39-dl-1_00009_mcl_mbr_abg_fmr.jpg` and links the supplied processed JPEG. The note distinguishes Dave's reported substantial quality loss from the still-unverified conversion command/log and batch extent. Probable Utrecht-only scope and multiple PDFs/shelfmarks are recorded as recollections, not established boundaries.

The present decision is to retain the derivatives with provenance, allowing a possible later comparison with higher-quality renditions. The dataset/paper should explain that the experimental files can differ from institution-hosted images; the reduced quality should not be attributed to Utrecht's originals. No historical log hunt, image reprocessing, classification change, or frozen-dataset replacement was performed.

The previous guide handoff remains valid. This addition needs Dave's quick wording review, not a new pre-publication reconstruction project.

</details>

<details>
<summary>Comment 7197856963 — November 26, 2026 at 9:36:03 AM MST</summary>

Source: [original comment](https://github.com/bballdave025/congenial-chainsaw-rmfb-html/pull/14#issuecomment-7197856963); author: `bballdave025`.

## Closeout review — November 26, 2026 (America/Denver)

Dave has requested that the remaining documentation issues be recorded for later work rather than repaired before this merge. This status supersedes the outstanding-task lists in the earlier description/comments; their historical evidence is preserved.

- [x] Fuller guide exported with Appendix A, original/cropped/annotated image00131 illustrations, and the dated visibility/context clarifications.
- [x] Wrapper scope explained separately from the frozen annotation ontology; the initial experiment excludes wrapper images, output, and scoring.
- [x] Historical source guide renamed, with an opening warning and historical-reference footer on all 19 PDF pages. The Word blue textbox works well.
- [x] Smallest J shortcut and October 3 internal date corrected; both Markdown helpers renamed.
- [x] Remaining issues recorded in [the deferred checklist](https://github.com/bballdave025/congenial-chainsaw-rmfb-html/blob/docs/binding-context-conventions-2026-11-08/docs/FIXME_TODO_outstanding_ontology_issues.md).
- [ ] Deferred: residual U-for-UCR and GNI caption text, Appendix source-ID/figure-number typos, punctuation, meaning-sensitive captions, historical source checks, and repository housekeeping.
- [ ] PR #15 follow-up: reconcile OIC descriptions in the extended Markdown helper. The stitching descriptions are already in the Smallest DOCX/PDF (PDF p5); ordinary ripgrep does not extract those formats. Start the follow-up branch with `docs/dev_notes/guide_and_ideas_for_pr_15_2026-11-26.md`.

**Model handoff:** fuller p13 now explicitly excludes DGS004518368 image00660 as an author-selected precaution. This supersedes the earlier comment's advice not to exclude it on shared DGS alone. Record the decision in the derived manifest while preserving the historical file; it does not prove the image is a wrapper. Carry wrapper exclusion into outputs/metrics and pin the merged ontology revision before training. These implementation steps have not been performed by this documentation review.

**Discussion record:** [consolidated checklist and original PR description/comments](https://github.com/bballdave025/congenial-chainsaw-rmfb-html/blob/docs/binding-context-conventions-2026-11-08/docs/dev_notes/pull_request_14_comments_2026-11-26.md).

Reviewed document commit `3a7e9059e9385ea03e8d88d21ea4e46a727073c4`. Fuller/historical/Smallest PDFs have 23/19/8 pages. XML parses with 21 active entries including the clear-selection control; the recorded legacy HTML backup blob matches. This closeout does not certify every source or visual classification.

No further guide polishing is requested for this bounded closeout. Merge remains with Dave; no merge, source-image change, model run, or paid compute was performed.

</details>
