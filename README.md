# Multimodal Deep Learning Framework for Breast Cancer Diagnosis and Molecular Subtyping

**Status: Pre-hackathon plan.** This repository holds my Final Year Project (FYP) design document, and will hold the code and results produced during the **Built with Claude: Life Sciences** hackathon (July 7–13, 2026).

## What this project is

Breast cancer has molecular subtypes (Luminal A, Luminal B, HER2-enriched, Triple-Negative) that matter enormously for treatment planning but are hard to tell apart from a mammogram alone. A 2025 published baseline (Ben Rabah et al., *Diagnostics* 2025) got 88.87% AUC overall but only 67%/74% AUC on the Luminal A/B distinction specifically — close to a coin flip. This project proposes a set of architectural changes (dual-view imaging, lesion-localized cropping, radiomics, gated fusion) to close that specific gap.

Full architecture, data pipeline, experimental design, and honest limitations are in the [complete project report](./BreastCancer_FYP_Report.pdf).

## Hackathon scope (this week)

The full plan is a 10-week Final Year Project. For the 7-day hackathon, the scope is deliberately narrow — see **Section 1.5** of the report:

- **E0**: reproduce the published baseline on a fixed patient subset
- **E1**: swap in a patient-wise split + EfficientNet-B3 backbone, same subset, and report the AUC delta

That's it for this week. Radiomics, gated fusion, and deployment are real parts of the FYP (Sections 3.3, 4.4, 6, 7) but are explicitly *not* part of this week's deliverable — they continue afterward as the rest of the 10-week timeline.

## Data

[CMMD](https://www.cancerimagingarchive.net/collection/cmmd/) and [TOMPEI-CMMD](https://www.cancerimagingarchive.net/analysis-result/tompei-cmmd/), both from The Cancer Imaging Archive (TCIA). Access requested via TCIA as of this writing.

## Repo contents

| File | What it is |
|---|---|
| `BreastCancer_FYP_Report.pdf` | Full design document (architecture, pipeline, ablation design, limitations) |
| `results/` | *(added during hackathon week)* E0/E1 results table, training logs |
| `src/` | *(added during hackathon week)* Data pipeline + training code |

## Author

Built by Anushree — final-year Computer Engineering student, University of Mumbai.
