# Binding context and visible information: classification addendum

Clarified by David BLACK on 2026-11-08.

## Scope

This addendum states the annotation conventions governing the current
RMMFB ruthlessly MVP experiments and publication. It explains the
procedure to apply to visible reuse. It does not establish a permanent
taxonomy: later ontology versions may revise the conventions with expert
input and a recorded rationale.

Historical annotations and frozen inventories retain their provenance.
Record accepted corrections in the derived dataset's decision record;
this clarification does not automatically rename or relabel existing files.

## General principle

Classify the visible reuse instance by its binding context and the way
information is exposed in the image. A single original information-bearing
writing surface can supply regions that are assigned different reuse
classes after incorporation into a binding. Sharing an original surface
does not require those regions to receive the same class.

For example, different regions of one folio side, or of the same side of
a bifolium, may appear as exterior cover material, an exposed underside,
and spine protection. Apply each relevant class to the context actually
visible. The number of applicable reuse classes is not a count of
independent source leaves or fragments.

When an image shows more than one binding-reuse class, use `mbr` with
the applicable subtype tags under the existing multiple-class convention.
The same host codex and known related views must remain grouped for
train/development/test assignment despite different subtype labels.

## Applications of the convention

| Visible reuse context | Classification procedure |
|---|---|
| A folded-back or turned-over corner of the cover exposes information on its underside | Use `ucr` for that exposed under-cover reuse. A tear or hole is not required. |
| Information from an earlier use is visible on or through the exterior cover surface | Use `orc`. Visibility through the surface, including bleed-through or corrosion where applicable, does not exclude ORC. |
| Information from an earlier use is visible on or through front/back matter within the guide's FMR scope | Use `fmr`; direct surface visibility is not required. |
| Visible reused material occupies the spine-protection context described in the guide | Use `spr` for that context. The shared origin of the material does not erase its binding role. |

These conventions concern information attributable to an earlier use.
Writing added as a title or other annotation for the current binding does
not establish reuse by itself. A spine visible in an image does not by
itself establish SPR: the existing guide distinguishes exterior cover
material from spine-protection material.

Do not infer a particular physical mechanism merely from the label.
Show-through, ink penetration, and corrosion need not be distinguishable
from the available image. Record uncertainty about the mechanism separately.

A fold, tear, or hole can reveal the same relevant under-cover context.
The current ontology uses UCR for that context rather than creating a
separate class for each exposure mechanism. This is the annotation rule
for this study; its application does not depend on demonstrating a
particular model-performance effect.

## Placement in the guides

Append this dated addendum after the existing content of each maintained
Word guide, then regenerate its corresponding PDF. This preserves the
class-by-class pages and the compact reference tables.

- `Simple_Classifications_-_1-or-2-pg_each.docx`
- `Simple_Classifications_-_1pg_each_-_resizes_to_show_MS_IDs.docx`
- `Smallest_Classification_Instructions_FHTW2025_read-print-able.docx`

The README and Markdown helpers link here, and `classifier.param` carries
a comment summarizing the convention. The legacy HTML presentation is
retained as historical material and is not being expanded with this addendum.
The Word/PDF files have not yet been regenerated with this addition.

## Related ontology rules

See [the README's multiple-class definitions](README.md#meaning-and-combinations-of-mcl-mbr-and-mmx)
for `mcl`, `mbr`, and `mmx`. This addendum introduces no new class IDs,
keyboard shortcuts, directory names, or filename tokens.
