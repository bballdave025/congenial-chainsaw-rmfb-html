# RMMFB guide consistency review — 2026-11-08

Status: documentation review completed; human image audit remains in progress.
Branch: `docs/binding-context-conventions-2026-11-08`.
PR: https://github.com/bballdave025/congenial-chainsaw-rmfb-html/pull/14

## Scope and authority

Reviewed the DOCX text and published PDF pages of all three named Word/PDF
pairs, both Markdown helpers, the README tables, and the active XML entries
in `classifier.param`. Page numbers below are PDF page numbers, counted from 1.
The review compared text, tables, shortcuts, captions, and proposal status;
it is not an expert reclassification of all illustrated manuscript images.

The source baseline is commit
[`c8402b403055774d9eb7732952ad13c80d92b83f`](https://github.com/bballdave025/congenial-chainsaw-rmfb-html/tree/c8402b403055774d9eb7732952ad13c80d92b83f).
This is the reviewed documentation snapshot, not a recovered original ontology
freeze date. See [provenance](ONTOLOGY_PROVENANCE.md).

Names used below:

| Short name | Reviewed file stem | PDF pages |
|---|---|---:|
| Fuller guide | `Simple_Classifications_-_1-or-2-pg_each` | 20 |
| Historical source guide | `Simple_Classifications_-_1pg_each_-_resizes_to_show_MS_IDs` | 18 |
| Smallest guide | `Smallest_Classification_Instructions_FHTW2025_read-print-able` | 8 |
| MVP helper | `shorter_fhtw2025_shortest_classify_helper.md` | — |
| Extended helper | `shortest_classify_helper.md` | — |

David's direction: use **`classifier.param` for current keyboard shortcuts**.
No executable XML class, key, token, or directory definition is changed by
this review. Corrections to Markdown reference tables follow the existing
configuration; DOCX/PDF edits and proposed renames remain for David.

## Findings and disposition

| ID | Location and evidence | Disposition |
|---|---|---|
| G01 | c8 continuation: historical source guide p9 says **B**; fuller guide p10 says **C**. c8 is C/`scg`; B is `mbr`. | Fuller C agrees with the c8 definition. Keep the older page as historical evidence under the requested outdated-instructions footer. |
| G02 | Fuller p3 repeatedly uses **U** for UCR, including “Y and U”; p6 says “Also U (red).” Historical source p5 has the latter. `classifier.param` assigns **R** to UCR and **U** to Unsure. | In the maintained fuller guide, use **UCR (R)** where that class is intended; remove the misleading shortcut. Keep U only when it genuinely means Unsure. Review image annotations as well as prose. |
| G03 | Fuller pp13–16, historical pp12–15, Smallest p2 and the old MVP helper use **Y** for c15 `gni`. XML uses **J**. | Resolved by David: **J**. README and both helper tables now follow XML. Update current Word/PDF headings, prose and the Smallest mnemonic; do not globally replace every Y in unrelated text. Historical source guide substance stays unchanged. |
| G04 | Fuller pp14–16 repeatedly says “general **in-situ** stuff” while discussing `gni`; also retains `Pick <didn't make a pick>`. | Replace with explicit current wording: “Use J (`gni`, general **not in situ** reuse) for the combined c11–c14 category.” Mark the individual old keys/definitions as historical. |
| G05 | Fuller p12 wrapper examples conflict about `mbr`: FamilySearch image39 says 4+F **without B** because it is one piece, while the St. Gallen partially unwrapped example says 4+F+**B**. Historical source p11 contains the same tension. | Record the ambiguity. David has chosen to exclude wrappers from this experiment and its prediction head, without changing the frozen ontology. This need not hold up the MVP; see the wrapper evidence below. |
| G06 | Fuller p11 / historical p10: G is an across-gutter view marker. G+F is **not B**; G+F+R is B. Fuller p2 also permits uncertain R/P alternatives for one piece without B. | Preserve both exceptions. The new context explanation and XML comment now avoid an unconditional “count tags” rule. |
| G07 | Both helper c8 rows said `Small_Connecting_or_Guard_Reuse`; fuller p9, Smallest p1 and XML use `Connecting_or_Guard_Reuse`. | Helper directory/display wording corrected. Keep `scg`; it is not an instruction to rename old image directories. |
| G08 | Extended helper c103 row said `Multiple_Mixed_Incl_Not_Binding`, contradicting its own Nov5 note and XML's **all not binding** meaning. | Row corrected to `Multiple_Mixed_But_All_Not_Binding`. No new `mmx` semantics introduced. |
| G09 | MVP helper omitted c112 `iac`; extended helper omitted c15 `gni`, c111 `fko`, and c112 `iac`, though XML and Smallest include them. | Missing current reference rows added; active keys are J, K, Z respectively. These markers/control categories are not automatically all model outputs. |
| G10 | Extended helper's c11–c14 looked like separate current choices; other guides combine them into c15. | Historical rows marked and explained; current c15 added. Current XML remains unchanged. |
| G11 | Extended helper's struck-through future-phenomena IDs differ from fuller p17 / Smallest p5. Its old proposed c60 `nbr` also collides with current c121 `nbr`. | Preserve the old proposal with an explicit warning and the crosswalk below. Do not apply old proposed IDs/tokens to current files or activate them by implication. |
| G12 | Helpers lacked the Smallest p1 / fuller p11 caveat that `abg` can concern OIC, not only reuse. | Added the caveat. `abg` by itself is not a positive binary reuse label. |
| G13 | Helper/README c122 directory capitalization differed from XML (`but` versus `But`). | Current Markdown reference spelling follows XML. Historical path strings remain historical; no filesystem rename performed. |
| G14 | Smallest p3 says it contains only study classes, but pp5–8 include future phenomena/ideas. Both old helper endings also describe earlier scope. | Helper scope notes updated. Suggested Smallest wording: “The preceding table records the study's classification scheme and associated controls; subsequent pages retain possible future extensions.” |
| G15 | Smallest p4 says **2026-10-13**; its repository update and README note are **2026-10-03**. | David should verify the intended internal note date. Do not infer or change the ontology lock date from it. |
| G16 | Both helper c9 rows had unclosed `<ins>` markup; several extended-helper proposal rows had unbalanced strike markup. | Markup repaired. Preserve the distinction between historical proposals and current settings. |

### Smaller proofreading and source-caption checks

- **Fuller p1:** the ORC definition has two clauses run together (“visible on
  the outside cover surface is visible through…”). Suggested wording:
  “Text, decoration, or illumination from an earlier use is visible on the
  exterior cover surface or through it from the other side.”
- **Fuller p1 / historical p1:** malformed Bamberg caption
  `Ba,berg+=+JV<Msc359_00073`. The historical page also records David's
  “Final verdict: `Bamberg_-_HVMsc359_00073`.” Use that recorded correction
  as the starting point; this review did not independently verify the catalogue.
- **Historical p5:** `Heidelberg_-_salVII73__z4_0000` appears incomplete.
  It is useful evidence for recovering a source, not a confirmed complete filename.
- **Fuller p6:** the center caption's **O** and its “No need for it to be small”
  wording should be checked against the colored regions before editing. It
  may refer to a different visible surface, so its position on a CWA page
  alone does not prove O should be W. Its **U-for-UCR** shortcut problem is
  independently established (G02).
- **Fuller p7 / historical p6:** `zLOC_-_MarcoPolo...` has an apparent stray
  `z`; “some n orange” should read “some in orange.” Confirm source spelling.
- **Fuller p9:** repeated “the the.”
- **Fuller p12:** “what I'm **not** thinking is actually W” may mean “**now**”;
  author check, because changing a negation can change the instruction.
  The image40 caption also adds **J** compared with the older guide; under
  the current configuration J means `gni`, not an old proposed OIC key.
- **Fuller p13 / historical p12:** `FamiliySearch` spelling in a source caption.
- Question marks, incomplete source labels, and draft wording remain in the
  illustrated guides. The historical source guide identifies **many** examples;
  it is not a complete, independently verified source catalogue.

### Things that are not new inconsistencies

- Omission of c5 from the fuller guide corresponds to the documented decision
  to omit `obr`; it is not evidence of a missing PDF page. Smallest c5 is struck out.
- `suh` is explicitly deprecated; its retained historical filename tokens
  should not become current targets. No need to delete those files.
- The tool's c125 Unsure option and the original 3331 forced-choice annotation
  protocol describe different things. Document both. `fko` conveyed partial
  qualitative uncertainty, not calibrated confidence.
- The historical source guide lacks c62 `apc`, which appears in the later
  fuller/Smallest lists. Preserve that as a version difference.
- DOCX text extraction can concatenate table cells or duplicate text-box
  content. Such extraction artifacts alone do not establish a stale PDF.

## Wrapper examples and current experiment scope

**User decision, November 8:** retain the frozen classification procedure,
exclude wrapper examples from the current derived experimental dataset,
and omit the wrapper prediction output. Whether the sparse examples would
harm learning is a hypothesis; the defensible stated reason is a bounded
scope with insufficient examples for this category. Do not present an
unperformed ablation as measured harm.

The actual example evidence is:

| Source / search key | What the guide says | Filename certainty |
|---|---|---|
| `FamilySearch_-_DGS004518368_00038` | 4+F+W+B in the depicted view; without W, caption says B would not be needed. | Image38 is explicitly identified in the caption; this is a search stem, not a recovered complete tagged filename. |
| `FamilySearch_-_DGS004518368_00039` | 4+F, **not B**, explicitly because one writing surface receives both labels. | Image39 is explicitly identified; complete tagged filename not recovered. |
| `FamilySearch_-_DGS004518368_00040` | Main wrapper example; also F and W/B, with J in the fuller caption. | Historical source guide explicitly prints this source stem. |
| St. Gallen, Stiftsbibliothek, **Cod. Sang. 692** | Closed side shown as wrapper **without reuse**; partially unwrapped view gets 4+F+B. | Codex identified in the historical caption. No image number or exact image filename recovered; do not invent one. |

The two apparently conflicting 4+F decisions are image39 and the partially
unwrapped Cod. Sang. 692 example. They may depend on an unstated distinction;
the review records the textual inconsistency without making a new binding judgment.

### Check against the actual 3331 inventory

The checked `consistentized_3331_dataset.txt` has **3,331 entries** and SHA-256
`f0088ea2580c2c77f8b559c43c1830f905c705db6142e1c7793692f77d6d5fd8`, matching
the completed image audit's inventory hash.

- **Zero** filenames have a standalone `wpr` classification token.
- **Zero** listed paths contain a `Wrapper_Reuse` directory.
- The three FamilySearch example stems above do **not** occur.
- No Cod. Sang. 692 filename was found by the codex spelling variants checked.
- The one listed file from DGS004518368 is
  `No_For_Binding_Reuse/FamilySearch_-_DGS004518368_00660_nbr.jpg`.
  It is a different image. Shared DGS does not establish that it depicts a wrapper,
  or even the same host volume; do not remove it solely for that reason.

This is evidence of **no explicitly labeled wrappers in the inventory**, not
proof that no unrecognized or differently labeled wrapper appears in the pixels.
Keep a wrapper flag during the existing visual review. If one is found, record
its source path, accepted identity, exclusion reason, reviewer and date in the
derived selection manifest. Exclude the image even if other positive labels
co-occur; simply dropping `wpr` would not satisfy the requested image exclusion.
Retain all original bytes and labels. No source image has been moved or deleted.

The annotation tool's c10/4/`wpr` remains unchanged. A separate experiment
configuration/target list should omit it; changing ontology XML to disable a
model output would conflate two different configurations. This PR records the
scope decision but does not claim that training code or a split manifest has
already been changed.

For overlapping prediction targets, a usual model head is one logit per target,
with per-target sigmoid scores and a multilabel binary cross-entropy loss.
PyTorch's [BCEWithLogitsLoss](https://docs.pytorch.org/docs/2.15/generated/torch.nn.BCEWithLogitsLoss.html)
combines sigmoid and binary cross-entropy numerically stably. Pass logits to
that loss; apply sigmoid when producing scores. A single softmax over all
subtypes forces competition and is not the usual multilabel formulation.
Define the actual target list separately from bookkeeping flags such as `fko`.

## Proposed coordinated filenames — not yet applied

| Existing stem/name | Proposed stem/name |
|---|---|
| `Simple_Classifications_-_1pg_each_-_resizes_to_show_MS_IDs.(docx/pdf)` | `RMMFB_Example_Source_Reference_HISTORICAL_2025-05-07.(docx/pdf)` |
| `shorter_fhtw2025_shortest_classify_helper.md` | `RMMFB_Classification_Reference_MVP_Binding_Reuse.md` |
| `shortest_classify_helper.md` | `RMMFB_Classification_Reference_Binding_Reuse_and_Future_Phenomena.md` |

The date identifies the historical source-guide DOCX revision, not the
experimental freeze. The extended helper includes reuse as well as future
phenomena; calling it an OIC-only guide would be misleading. The clearer name
also avoids suggesting that every row is an active classification target.
Update links and first-line titles in the same rename commit. Do not rename
image files or their historical classification directories as a side effect.

### Every-page footer for the historical source guide

> HISTORICAL SOURCE REFERENCE — CLASSIFICATION INSTRUCTIONS OUT OF DATE.
> Current instructions: Simple_Classifications_-_1-or-2-pg_each.pdf

Use a legible bold footer, with a link to the current guide if practical.
Check every Word section and any different first-page/even-page footer settings;
then inspect the exported PDF to ensure the notice appears on every page.
Preserve the historical body instructions and source captions.

### Scope wording for the extended helper

> Other interesting phenomena were deliberately noted during the original
> annotation, using `oic`, `mcl`, or `mmx` as applicable. These provide a useful
> candidate pool for later work; completeness for each phenomenon has not been
> independently measured. A missing marker is not a verified negative label.
> The current stitching review adds a separate annotation layer without
> rewriting the frozen reuse inventory.

This expresses the intended care without an invented percentage or a promise
that all stitching, manicules, fingerprints, or other phenomena were captured.

### Historical extension crosswalk

The newer proposal is in fuller p17 and Smallest p5. These are candidate
phenomena, not activated XML definitions or a mandate to annotate them now.

| Phenomenon | Older extended helper | Newer guide proposal |
|---|---|---|
| Any stitching | c51 / stc | c50 / stc |
| Stitching levels 1, 2, 3 | c52–c54 / st1–st3 | c51–c53 / st1–st3 |
| Manicule | c55 / man | c54 / man |
| Non-manicule nota bene | c56 / nmn | c55 / nmn |
| Fingerprint | c57 / fgp | c56 / fgp |
| Hair on parchment | c58 / hop | c57 / hop |
| Visible watermark | c59 / vvw | c58 / vvw |
| Reuse not for binding | c60 / **nbr** | c59 / **nfb** |
| Corrosion through surface | c74 / igt, within older c71–c74 grading proposal | c60 / igt |
| Squished bug remains | Absent | c61 / sbr |
| Alphabet/pen trials/counting | Absent | c62 / apc |

## Recommended placement and paste-ready text

Use an **in-document Appendix A** in the fuller illustrated guide only.
It explains an existing organizing principle and belongs with the examples.
An in-document addendum would also work, but “appendix” better avoids suggesting
a newly adopted annotation rule. A separate DOCX/PDF addendum creates a second
file readers must locate and keep synchronized. The repo Markdown explanation
can remain a convenient linked reference without becoming that second Word guide.

The following is the proposed text to paste after the existing pages.
The dated scope sentence is essential: this is an explanation of the locked
procedure for this experiment, not a claim that every older document was identical.

---

### Appendix A — Binding context and a shared original writing surface

*Explanatory note recorded 8 November 2026. This appendix describes the
annotation procedure already adopted for the current RMMFB MVP experiments
and publication. It does not introduce new classification rules.*

Classification follows the reuse context visible in the image. A single
original information-bearing writing surface—such as one side of a folio
or the same side of a bifolium—can occupy several different positions after
incorporation into a binding. Regions from that surface can therefore receive
different reuse classifications. Several applicable classes do not imply
several original leaves or fragments.

Apply the existing class definitions to the visible regions:

- **Outside-cover reuse (ORC):** earlier information is visible on or through
  the exterior cover surface. Writing added for the present binding, such as
  its title, does not by itself establish reuse.
- **Under-cover reuse (UCR):** earlier information is exposed in the under-cover
  context. A turned-back corner can reveal it; a tear or hole is not required.
- **Spine-protection reuse (SPR):** reused material appears in the
  spine-protection context specified in the SPR instructions. Merely seeing
  a book's spine is insufficient.
- **Front/back-matter reuse (FMR):** earlier information can qualify when
  visible through the material, as well as directly on its surface, within
  the FMR definition.

Visibility does not necessarily establish how the information became visible.
Show-through, ink penetration, and corrosion may be difficult to distinguish
from a digitization. Uncertainty about that mechanism can be recorded
separately from the assigned context label.

**Example: FamilySearch DGS008279842, image 00131.** The annotated regions
illustrate ORC, UCR, and SPR in different visible contexts of what is interpreted
as one original writing surface. The accepted audit annotation retains `fko`
and `mbr` alongside `orc`, `ucr`, and `spr`.

[include annotated image here]

*Figure A1. Context-dependent classifications in DGS008279842, image 00131.
The marked regions distinguish visible uses of the material, not a count of
independent source leaves.*

Apply the guide's existing multiple-class conventions and specific exceptions.
For example, UCR/SPR alternatives for one uncertain piece do not alone warrant
`mbr`; nor does the across-book-gutter marker count as an additional reuse
subtype. This appendix does not replace those more specific instructions.

These conventions fix how this study's annotations are interpreted. Any
expected learning or generalization benefit is a separate research hypothesis,
not a demonstrated consequence of the ontology. Later studies may revise the
ontology explicitly, preserving the version used for each experiment.

---

Editorial note outside the appendix: the supplied string
`fko_mbr_orc_ucr_sprucr` appears to join `spr` and a second `ucr`. The accepted
**set** is `fko`, `mbr`, `orc`, `ucr`, `spr`. Do not create a `sprucr` token or
silently rename a historical file. Final derived filenames follow the recorded
normalization convention.

## Suggested repository About description

> RMMFB classification ontology and illustrated annotation guides, maintained in Word with PDF exports, XML classifier configuration, and concise Markdown references.

David will update the About field. The legacy HTML presentation remains
historical, explicitly superseded by the Word-to-PDF workflow.

## MVP boundaries and publication placement

This audit earns its place in the MVP because it addresses duplicate imagery,
source-identifier mistakes, conflicting labels, and split integrity. It should
have an exit condition: resolve the prioritized exact/conflicting cases and
relevant near-duplicate candidates, record decisions and exclusions, produce
the derived manifest, and verify host-group separation. It is not a mandate
to rebuild the entire ontology or revisit every historical judgment.

The filename edit-distance finding belongs in the audit record and a brief
methods/data-curation paragraph: removing classification suffixes and comparing
similar source identifiers found identical imagery masquerading as distinct
records after a DGS typo. Give EG002 as a concrete case. A technical appendix
can explain normalization, insertion-heavy flags, image-hash confirmation,
and source lookup. The portfolio can describe the full evidence trail.
No need to implement keyboard-neighbor error models for this MVP.

Stitching is a bounded secondary demonstration if it fits the publication
schedule. Fast annotation makes it plausible, but does not measure the time
needed for controlled training, review, and analysis. Keep raw images and
Dave's painted annotations separate; keep the same host codex and related
views in one split. For the sequential-transfer comparison, the reuse checkpoint
must not already have trained on the stitching-test host groups. Freeze the
reuse checkpoint, compare it with the original public initialization under the
same stitching protocol, and describe the learning benefit as a hypothesis.
Human/model heatmap agreement is supporting localization evidence, not proof
that a model's entire decision process is correct. Additional phenomena remain
future work. Wrapper exclusion limits the current study's scope; it is not
proof that wrappers are intrinsically unsuitable for later modeling.

## Before merging

- David: append Appendix A to the fuller DOCX, insert the annotated example,
  correct its current shortcut/prose issues, and export/inspect the PDF.
- David: rename the historical DOCX/PDF, apply the footer to every page,
  and retain their historical body content.
- David: correct Smallest's J shortcut and scope note; check its internal date.
- David: apply the two proposed helper renames if accepted and update links.
- No need to settle the wrapper taxonomy for this MVP; retain the discrepancy
  and record its experimental exclusion. Do not delete frozen images.
- Record the actual merged commit used by experiments after these edits.
  The old freeze date remains unverified; the new explanation does not reset it.

Assistant changes completed in this PR: review and appendix draft; revised
placement/provenance notes; current Markdown table corrections; historical
proposal warnings; wrapper inventory finding and scope record; comments in
XML only. DOCX/PDF binaries, image bytes, training code and split manifests
were not edited.

Validation completed: both helper tables contain all 20 active non-clear XML
entries and agree with XML on each directory, shortcut, and filename token.
Parsed non-comment XML is unchanged. Local Markdown links resolve, repaired
HTML wrappers balance, and `git diff --check` passes. The inventory check used
the audit-matching SHA-256 above. This validation does not certify every visual
example or resolve the historical wrapper caption discrepancy.
