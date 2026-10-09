# Featured Case — Workplace Drama Digital Forensic Investigation

**Case type:** Simulated forensic examination of a workplace-threat scenario. **Training data only.**

## Executive summary

The completed student report describes examination of a forensic disk image using **Autopsy 4.22.1**. It correlates a presentation, a document, and a chat artifact with reported system activity to develop an investigative narrative. The submitted report also documents an evidence-handling log, methodology, a timeline, and limitations. The report's interpretations are **not independently revalidated** by this portfolio package.

## Examination methodology (as reported)

1. Downloaded two assigned compressed evidence archives.
2. Extracted archives using **7-Zip 23.01** and organized files locally.
3. Created an Autopsy case called `Final` and disabled selected ingest modules.
4. Added a disk image called `LoneWolf.E01` in the report and completed ingest to 100%.
5. Reviewed documents, communications, and timestamps to answer case questions.
6. Produced a structured forensic report with three labeled exhibits.

> **Source discrepancy:** The assignment calls for `WorkPlace.E01`, but the submitted report names `LoneWolf.E01`. Without the original evidence manifest, these cannot be assumed to be identical. The portfolio preserves the discrepancy.

## Reported timeline

| Event | Time (UTC) | Cited source within report |
| --- | --- | --- |
| Earliest activity indicator | 2018-03-29 02:37 | `AIRPORT INFORMATION.docx` timestamp |
| Latest activity indicator | 2018-04-06 04:36 | OneNote `.bin` timestamp |

These timestamps are the **reported examination window**, not proof of actual power-on or shutdown times.

## Key artifacts

| Exhibit | Artifact | Interpretation in report |
| --- | --- | --- |
| [A](../../evidence/workplace-drama/README.md#exhibit-a) | `Operation 2nd Hand Smoke.pptx` | Presentation relevant to the scenario's planning narrative |
| [B](../../evidence/workplace-drama/README.md#exhibit-b) | `The Cloudy Manifesto.docx` | Document analyzed for contextual information |
| [C](../../evidence/workplace-drama/README.md#exhibit-c) | Brother Chat (Google Docs) | Communication artifact correlated with other evidence |

## Limitations and examiner caution

- Findings are limited to accessible artifacts from the supplied training image.
- Some cached or binary fragments could not be fully reconstructed.
- References to cloud services do **not** establish that remote data was collected.
- The report includes inconsistent custody dates and an image filename discrepancy.
- No original disk image, independent hash validation, or full Part B answers are published here.

See [selected exhibit previews](../../evidence/workplace-drama/README.md) and [documentation quality notes](../../docs/evidence-quality-and-limitations.md).
