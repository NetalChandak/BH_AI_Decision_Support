# NoRA Mobility 2030 — Evidence Package

## Project #1 — AI-supported future mobility estimation

### Purpose

This repository documents an evidence-led, scenario-based analysis of plausible 2030 mobility outcomes for NoRA, and compares the independent working estimate with stated NoRA/CMP mobility ambitions and comparable planning targets.

The package is designed to be auditable: every material number is labelled as a **source fact**, **planning target**, **model assumption**, **calculated output**, or **sensitivity range**.

> **Important:** The 2030 values in this package are analytical working estimates, not approved NoRA targets and not outputs from a detailed NoRA travel-demand model.

## Core question

> For 2030, what is a plausible range for public transport mode share and internal trips by sustainable modes, considering historical/current conditions, future estimates, development phasing and growth factors?

## Key outputs

| Metric | 2030 working estimate | Sensitivity range |
|---|---:|---:|
| Public transport mode share | **25–30%** | **~19–35%** |
| Internal trips by sustainable modes (PT + walking + micromobility) | **~45%** | **~35–55%** |
| Trips internalised within NoRA | **~55–60%** | **~50–65%** |
| Population | Phasing-dependent | **~2.5–3.5M** |

## Evidence hierarchy

1. Primary project source documents
2. Official government / institutional data
3. Authoritative external research / benchmarks
4. Comparable-city evidence
5. Explicit analytical assumptions
6. AI-generated hypotheses requiring validation

## AI traceability

AI was used to accelerate source extraction, evidence organization, scenario development, sensitivity analysis and comparison. AI output is **not treated as evidence by itself**. A claim is accepted into the model only when it is supported by an identified source or explicitly labelled as an assumption.

The audit trail follows:

**Prompt → Source/Input → AI Output → Analyst Review → Final Model Decision**

## Repository map

- `01_Project_Context/` — question, scope and intended business use
- `02_Source_Evidence/` — source register and evidence cards
- `03_Historical_Baseline/` — baseline evidence and data limitations
- `04_Methodology/` — modelling logic and assumptions
- `05_2030_Model/` — working estimates and calculation workbook
- `06_Sensitivity/` — conservative/base/accelerated scenarios
- `07_Comparison/` — comparison with NoRA/CMP/RUA targets
- `08_AI_Traceability/` — selected prompts and responses needed to reproduce the workflow
- `09_QA_Validation/` — QA checklist and limitations
- `10_Final_Output/` — executive summary and evidence-package narrative

## Source confidentiality

The original client/project PPTX/PDF files are **not copied into this repository by default**. The NoRA source deck is approximately 48 MB and the RUA CMP PDF is approximately 161 MB; more importantly, project documents may be subject to client confidentiality restrictions. The repository therefore uses source names, slide/page references and extracted evidence rather than redistributing source files.

See `02_Source_Evidence/source_register.md` and `02_Source_Evidence/source_handling.md`.
