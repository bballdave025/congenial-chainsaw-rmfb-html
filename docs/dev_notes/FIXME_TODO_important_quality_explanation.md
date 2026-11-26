# FIXME / TODO — Important explanation of derived-image quality

Recorded: 8 November 2026, from David BLACK's audit observations.
Status: **retain the example and document the processing difference; recover
precise batch provenance later.** This note does not change its classification.

## Example to keep track of

Exact filename:

```text
UnivUtrecht_-_F-oct-39-dl-1_00009_mcl_mbr_abg_fmr.jpg
```

The checked 3331 inventory records it as:

```text
./Multiple_Binding_Reuse_Classes/UnivUtrecht_-_F-oct-39-dl-1_00009_mcl_mbr_abg_fmr.jpg
```

[View Dave's supplied processed JPEG](assets/UnivUtrecht_-_F-oct-39-dl-1_00009_mcl_mbr_abg_fmr.jpg).
This linked file is the supplied dataset-derivative example, not a download
of the holding institution's original/master image. It is included here as
processing evidence and is not a new training example.

The supplied attachment is an RGB JPEG, 834 × 1389 pixels, 101,641 bytes.
Its SHA-256 is:

```text
86fbea66e919d55526fbb435df7994452e0ee36655f2c38fea580c1f31de0b87
```

These measurements identify the supplied attachment. Matching its filename
to the inventory does not by itself establish byte identity with every local
copy of the dataset or with an institution-hosted image.

## Reported processing history and uncertainty

Dave identifies this image as belonging to one batch of **PDF → PNG → JPG**
conversions that deviated from the usual image-processing workflow. He reports
that the deviation substantially reduced image quality relative to what the
normal workflow or higher-quality source material would have provided.

Dave recalls having previously traced this to a particular command in a
particular log. That command, its parameters, and the log location have not
been recovered or verified for this note. The sequence of file formats alone
does not identify the cause or magnitude of the loss.

Dave believes the affected batch contained only University of Utrecht material,
and likely included more than one codex, shelfmark, or PDF. Both the
institution-only boundary and the full set of affected records remain to be
checked. Do not mark all Utrecht images as affected solely from their prefix,
and do not assume this one shelfmark exhausts the batch.

## Why retain it

Dave's present decision is to retain these lower-quality derivatives in the
dataset, with their processing history documented. They may support a later
comparison with higher-quality renditions of the corresponding images.
This possible comparison is future work, not an experiment already performed
or a demonstrated benefit of retaining degraded inputs.

Preserve the frozen files, historical filenames, and labels. Do not silently
replace them with a new conversion or apply restoration/sharpening as part of
this documentation change. Any later higher-quality version should be recorded
as a related rendition, with its own provenance and file hash.

If paired renditions are used later, keep them—and their other host-codex views—
in the same train/development/test group. Different resolutions or processing
histories do not make views of the same object independent evaluation examples.

## Explanation needed in the dataset description and paper

The files supplied to a model can be locally processed derivatives rather
than the same digital files hosted by the holding institution. The methods
should identify the actual experimental inputs and disclose this exceptional
conversion batch. Readers should not interpret a degraded training example
as evidence that the institution's digitization has the same limitations.

Provisional wording, to be checked against the final manifest:

> Our experimental image files include locally generated derivatives of
> institution-provided material. During curation, we identified a batch of
> PDF-to-PNG-to-JPEG conversions that departed from our usual workflow and,
> according to the curator's review, introduced substantial quality loss.
> These derivatives are retained and flagged for a possible later comparison
> with higher-quality renditions. Their appearance should not be taken as
> representative of the quality of the files hosted by the holding institution.
> The precise command and complete affected batch remain under provenance review.

If the batch is resolved before publication, replace the final sentence with
the verified command/log reference and affected-image count. Do not claim a
quantified quality reduction without a corresponding measurement.

## Deferred follow-up

- [ ] Recover the previously identified command, log path, and relevant lines;
      record the software/version and conversion parameters where available.
- [ ] Establish the affected batch across PDFs/shelfmarks, recording evidence
      for membership rather than assigning it from the institution prefix.
- [ ] Link source PDFs/images and available higher-quality renditions to the
      actual experimental files; retain hashes and dimensions for each rendition.
- [ ] Add a processing-quality/provenance flag to the derived manifest, with
      unknown values left explicit until the batch is verified.
- [ ] Carry the verified explanation into the dataset methods/limitations;
      leave any paired quality experiment as later work unless explicitly scoped.

No historical log search, batch reconstruction, image replacement, or new
classification decision was performed as part of this note.
