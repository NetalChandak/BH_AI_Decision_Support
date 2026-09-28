# QA checklist

## Source QA

- [x] Every material source-derived number has a source ID.
- [x] Source-derived values are distinguished from model outputs.
- [x] RUA/CMP figures are treated as benchmark inputs for comparison, not NoRA forecast inputs.
- [x] Long-term NoRA targets are not labelled as 2030 observed outcomes.

## Numerical QA

- [x] External car share is residual to PT share in the simplified comparison.
- [x] RUA internal sustainable share is checked as 54% + 30% + 16% = 100%.
- [x] Sensitivity ranges contain the working estimates.
- [x] Population sensitivity is documented as a context range, not a precise occupancy forecast.

## Model QA

- [x] Assumptions are editable and documented.
- [x] Scenario drivers are documented.
- [x] Uncertainty is expressed as ranges.
- [x] No standalone walking/PRT/micromobility NoRA 2030 values are invented.

## AI QA

- [x] Material prompts are recorded.
- [x] Material responses are recorded in curated form.
- [x] AI-generated values are labelled as modelled unless directly sourced.
- [x] Human/analyst review points are documented.

## Validation still required

- [ ] Formal NoRA travel-demand model
- [ ] Calibrated trip generation
- [ ] Network assignment / capacity testing
- [ ] Approved phasing and occupancy assumptions
- [ ] Detailed walking/PRT/micromobility mode-choice inputs
