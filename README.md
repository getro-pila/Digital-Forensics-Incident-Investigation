# Digital Forensics & Incident Investigation

**Four training investigations | Autopsy 4.x | Forensic image analysis | Artifact recovery | Timeline reconstruction | Evidence reporting**

> **Portfolio overview:** A consolidated collection of digital-forensics exercises from NOS 210, *Digital Forensics & Investigations*, at Clover Park Technical College. The featured case is a documented examination of the fictional **Workplace Drama** training image. The remaining case pages describe assigned examination workflows; independent completion evidence for those exercises has not yet been supplied for publication.

## Executive overview

Digital forensics is more than recovering files: an examiner must explain **what the evidence shows, where it was found, how it was processed, and what cannot be concluded**. This project illustrates an end-to-end workflow: preparing forensic images, examining file systems, recovering artifacts, reconstructing activity, and communicating findings through a structured report.

**Featured case — Workplace Drama:** A simulated workplace-threat investigation in which document and communication artifacts were correlated with an activity timeline. The submitted report records three principal exhibits, an examination methodology, limitations, and an evidence-handling log. This is a **training scenario**, not a real-world allegation.

## Investigation portfolio

| Case | Examination focus | Evidence status |
| --- | --- | --- |
| [01 — Disk image & file recovery](cases/01-image-recovery/README.md) | E01 image loading, file-system navigation, export | Lab procedure provided; no separate completed screenshots verified |
| [02 — Rhino data carving](cases/02-rhino-data-carving/README.md) | USB image, deleted file identification, recovered diary | Lab procedure provided; no separate completed screenshots verified |
| [03 — Arson timeline & tagging](cases/03-arson-timeline-analysis/README.md) | Tagging, timeline views, document examination | Lab instructions provided; no completed case screenshots verified |
| **[04 — Workplace Drama (featured)](cases/04-workplace-drama/README.md)** | Image ingestion, timeline, artifact correlation, forensic reporting | **Completed student report supplied; three exhibit screenshots included** |

## Featured case: documented findings

| Area | Reported observation | Forensic relevance |
| --- | --- | --- |
| Examination platform | Windows 10 Enterprise LTSC VDI, Autopsy 4.22.1, 7-Zip 23.01 | Reproducible tool and environment context |
| Source image | `LoneWolf.E01` named in the completed report | Source identity **requires reconciliation** with the assignment's `WorkPlace.E01` |
| Activity window | 2018-03-29 02:37 UTC to 2018-04-06 04:36 UTC | Reported earliest and latest activity indicators, not independently revalidated |
| Exhibit A | `Operation 2nd Hand Smoke.pptx` | Planning-related presentation identified in training image |
| Exhibit B | `The Cloudy Manifesto.docx` | Document examined for contextual relevance |
| Exhibit C | `Brother Chat` (Google Docs) | Communication artifact considered alongside documents |

See [featured case analysis](cases/04-workplace-drama/README.md) and [evidence gallery](evidence/workplace-drama/README.md).

## Examination workflow

```text
Training evidence archives
          |
          v
7-Zip extraction / evidence organization
          |
          v
Autopsy case creation + disk image ingest
          |
          v
File-system / deleted-file / document review
          |
          v
Artifact tagging + timestamp correlation
          |
          v
Evidence exhibits + limitations + report
```

## Skills demonstrated and documented

- **Autopsy-based forensic examination:** image ingestion, navigation, and artifact identification.
- **Evidence interpretation:** correlating recovered documents and communications with a timeline.
- **Report writing:** methodology, evidence handling, exhibits, and investigative limitations.
- **Integrity awareness:** differentiating documented hashes and dates from independently verified values.

## Publication and evidence ethics

This repository contains **selected, low-detail exhibit previews** from a student's own report. It intentionally excludes raw disk images, recovered private documents, detailed threat-planning content, instructor-distributed case materials, and the original report. No evidence was collected from live third-party systems. Screenshot previews are illustrative of the submitted report, not independent verification of image hashes or custody records.

**Known documentation discrepancies:** The source image is labeled `WorkPlace.E01` in the assignment but `LoneWolf.E01` in the student report. The report header is dated March 2026, while some custody entries say March 2028. These are disclosed, not silently corrected. See [quality notes](docs/evidence-quality-and-limitations.md).

## Tools

[Autopsy](https://www.autopsy.com/) · [The Sleuth Kit](https://www.sleuthkit.org/) · 7-Zip · Windows PowerShell · HashCalc (reported)

**Author:** Getro Pila · **Context:** NOS 210 academic training portfolio
