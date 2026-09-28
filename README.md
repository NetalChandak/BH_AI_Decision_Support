# BH AI Decision Support

## Evidence-Backed AI for Future Planning & Decision Support

Future-facing business and planning decisions often rely heavily on **human judgment, assumptions, and expert experience**. These remain essential, but the underlying evidence, historical precedents, assumptions, and alternative scenarios are not always assembled consistently or transparently.

This project explores how an **AI-supported decision framework** can help consultants make better-informed future predictions and business decisions by combining:

- Historical project information
- Internal organizational knowledge
- External research and comparable cases
- Explicit assumptions
- Scenario and sensitivity analysis
- Evidence-backed reasoning
- Human professional judgment

The objective is not to replace consultant judgment or formal analytical models.

The objective is to make the reasoning behind future-facing decisions **more evidence-based, transparent, traceable, and reproducible**.

---

## The Core Question

Instead of asking only:

> **“What do we think will happen in the future?”**

the proposed approach asks:

> **“Based on historical evidence, current information, comparable cases, project characteristics, and alternative scenarios, what are the plausible outcomes — and what factors drive them?”**

---

## Proposed AI Decision-Support Workflow

```text
Internal Knowledge + Historical Projects + External Evidence
                           │
                           ▼
                    Analysis Agent
                           │
                           ▼
             Evidence & Assumption Extraction
                           │
                           ▼
               Scenario / Sensitivity Analysis
                           │
                           ▼
                Evidence-Backed Estimate
                           │
                           ▼
                    Human Review
                           │
                           ▼
                   Decision Support
```

The AI acts as an **analysis accelerator** rather than the final decision-maker.

### AI can support

- Finding relevant historical evidence
- Extracting planning assumptions and targets
- Identifying comparable cases
- Organizing evidence
- Identifying missing information
- Generating alternative scenarios
- Performing sensitivity analysis
- Comparing model outputs with existing plans
- Maintaining evidence and assumption traceability

### Human / Consultant remains responsible for

- Defining the business question
- Determining which evidence is relevant
- Reviewing assumptions
- Challenging AI-generated estimates
- Applying project and domain expertise
- Validating results against formal models
- Making the final recommendation or decision

---

# Validation Through Real Mobility Planning Cases

The approach is demonstrated through two mobility-planning case studies.

## Project 01 — NoRA Mobility 2030

### Question

What could NoRA's mobility outcomes look like around 2030 when considering:

- Riyadh's existing mobility baseline
- Long-term NoRA mobility ambitions
- Public transport development
- Transit-oriented development
- Parking and demand-management policies
- Development phasing
- Behavioral adoption
- Population uncertainty

### Analytical approach

```text
Current Baseline
      ↓
Long-Term Planning Direction
      ↓
NoRA Structural Advantages
      ↓
Infrastructure & Policy Assumptions
      ↓
Behavioral Adoption
      ↓
2030 Working Estimate
      ↓
Sensitivity Range
```

### Current working outputs

| Metric | 2030 Working Estimate | Sensitivity Range |
|---|---:|---:|
| Public transport mode share | **25–30%** | **~19–35%** |
| Internal trips by sustainable modes | **~45%** | **~35–55%** |
| Trips internalized within NoRA | **~55–60%** | **~50–65%** |
| Population | Phasing dependent | **~2.5–3.5M** |

These values are **analytical working estimates**, not approved project targets or outputs from a formal travel-demand model.

See: `Project_01_NoRA/`

---

## Project 02 — RUA / King Salman Gate

Project 02 tests a different analytical situation.

Rather than building an estimate primarily from a city baseline and future drivers, the RUA analysis starts with **existing project modal-split planning targets** and stress-tests them under alternative future conditions.

### RUA planning baseline

Normal conditions:

| Mode | RUA Planning Target |
|---|---:|
| External Public Transport | **60%** |
| External Car | **40%** |
| Internal Walking | **54%** |
| Internal PRT | **30%** |
| Internal Micromobility | **16%** |

Ramadan external conditions:

| Mode | RUA Planning Target |
|---|---:|
| Public Transport | **75%** |
| Car | **25%** |

### Scenario analysis

| Mobility Measure | RUA Target | Conservative | Base / Expected | Accelerated |
|---|---:|---:|---:|---:|
| External PT — Normal | 60% | 60% | **65%** | **70%** |
| External Car — Normal | 40% | 40% | **35%** | **30%** |
| External PT — Ramadan | 75% | 75% | **78%** | **82%** |
| External Car — Ramadan | 25% | 25% | **22%** | **18%** |
| Internal Walking | 54% | 54% | **55%** | **57%** |
| Internal PRT | 30% | 30% | **30%** | **29%** |
| Internal Micromobility | 16% | 16% | **15%** | **14%** |

The **RUA Target** column is source-derived.

The Conservative, Base / Expected, and Accelerated values are **analytical scenario assumptions** used to stress-test the planning targets.

See: `Project_02_RUA_King_Salman_Gate/`

---

# Two Different Decision-Support Patterns

The two projects intentionally demonstrate different uses of AI-supported analysis.

| | Project 01 — NoRA | Project 02 — RUA |
|---|---|---|
| Starting point | Limited project-specific historical data | Existing planning targets |
| Main question | What could 2030 look like? | How might existing targets vary under alternative conditions? |
| Approach | Baseline → drivers → estimate | Target → scenario stress-test |
| AI role | Build and challenge a working estimate | Stress-test an existing assumption |
| Output | Estimate + sensitivity range | Conservative / Base / Accelerated scenarios |

Together they demonstrate that the same evidence-based AI workflow can support different types of future-facing planning questions.

---

# Evidence-to-Decision Framework

A key principle of this repository is that **every important number should have a clear classification**.

| Classification | Meaning |
|---|---|
| **Source Fact** | Directly supported by a source |
| **Planning Target** | Stated target or ambition in project material |
| **Model Assumption** | Assumption introduced for analysis |
| **Calculated Value** | Arithmetic or model-derived result |
| **Model Output** | Result generated from assumptions and methodology |
| **Sensitivity Range** | Range created by changing key assumptions |

This prevents AI-generated estimates from being presented as source-derived facts.

---

# Repository Structure

```text
BH_AI_Decision_Support/
│
├── README.md
│
├── Project_01_NoRA/
│   ├── 01_Project_Context/
│   ├── 02_Source_Evidence/
│   ├── 03_Historical_Baseline/
│   ├── 04_Methodology/
│   ├── 05_2030_Model/
│   ├── 06_Sensitivity/
│   ├── 07_Comparison/
│   ├── 08_AI_Traceability/
│   ├── 09_QA_Validation/
│   └── 10_Final_Output/
│
└── Project_02_RUA_King_Salman_Gate/
    ├── 01_Project_Context/
    ├── 02_Source_Evidence/
    ├── 03_RUA_CMP_Baseline/
    ├── 04_Methodology/
    ├── 05_Scenario_Model/
    ├── 06_Sensitivity/
    ├── 07_Comparison/
    ├── 08_AI_Traceability/
    ├── 09_QA_Validation/
    └── 10_Final_Output/
```

Each case study preserves the chain from:

```text
Source Evidence
      ↓
Historical / Planning Baseline
      ↓
Assumptions
      ↓
Methodology
      ↓
Scenario Model
      ↓
Sensitivity Analysis
      ↓
Comparison
      ↓
QA / Validation
      ↓
Decision-Support Output
```

---

# AI Traceability

Selected prompts and responses are retained where they materially influenced the analysis.

The objective is **not to store a raw AI conversation dump**.

Instead, the repository records important analytical decisions as:

```text
Prompt
   ↓
Evidence / Inputs
   ↓
AI Response
   ↓
Human Review / Challenge
   ↓
Accepted or Revised Assumption
   ↓
Final Analytical Output
```

This makes it possible to understand not only **what the AI produced**, but also **how the result evolved**.

---

# Important Limitations

The analyses in this repository are intended for **decision support and scenario exploration**.

They should not be interpreted as replacements for:

- Formal travel-demand models
- Network and capacity modelling
- Approved project forecasts
- Engineering analysis
- Client-approved planning targets
- Professional/domain judgment

Where formal models or additional evidence become available, the AI-supported estimates should be validated and updated accordingly.

---

# Intended Outcome

The broader goal is to demonstrate a reusable consulting workflow:

> **Evidence + AI Analysis + Scenario Testing + Human Judgment → Better-Informed Decisions**

The value of the approach is not simply generating a prediction.

It is making the assumptions, evidence, uncertainty, and reasoning behind that prediction **visible, challengeable, and reproducible**.
