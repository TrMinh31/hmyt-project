<img width="778" height="138" alt="image" src="https://github.com/user-attachments/assets/264a7c19-5626-410d-8605-bc0000b17149" /># Progress Test 2 — <nhom15> — <topic_slug>

- Fork: <https://github.com/TrMinh31/hmyt-project> · Branch: gd5-proposed-model
- Members (student ID or alias) and roles:
- 202414856: research, EDA and model testing
- 202414831: research, data preparation and evaluation
## A. Literature review and research gaps

### A1. Search strategy
| Source (PubMed, Scopus, IEEE Xplore, Google Scholar…) | Keywords / query | Year range | No. of hits | No. kept |
|PubMed|Polypharmacy AND fall risk|2020–2026|295|10|

Inclusion / exclusion criteria:
- Inclusion: Focusing on effects of polypharmacy on increasing fall-risk among the elderly. Bonus attention for papers regarding anticholinergic burden and drug-drug interactions.
- Exclusion: Papers with any mentions on specific conditions (Diseases, disorders).

### A2. Literature matrix (≥ 10 papers, preferably from the last 3–5 years)
| # | Paper (authors, year) | DOI / link | Dataset (n, source) | Method | Main result (metric, value) | External validation? (yes / no) | Main limitation |
|---|---|---|---|---|---|---|---|
| 1 | Ramos et al. (2023). Effect of polypharmacy and FRIDs on falls among Brazilian older adults: The SABE cohort study | https://doi.org/10.1016/j.archger.2023.105127 | n = 2,387; SABE cohort, São Paulo, Brazil (2000–2006). |  Longitudinal observational study; Generalized Estimating Equations (GEE)| ≥2 FRIDs associated with falls: OR = 1.51 (95% CI: 1.16–1.96). Polypharmacy was not independently associated with falls after adjustment.|No|Medication dosage and administration frequency were not considered; recall bias from self-reported falls; unable to identify which FRID classes contributed most to fall risk. |
| 2 | Dinh et al. (2021). Are Anticholinergic Symptoms a Risk Factor for Falls in Older General Practice Patients With Polypharmacy? Study Protocol for the Development and Validation of a Prognostic Model. | 10.3389/fphar.2020.577747 | n = 1,699 planned participants: RIME (1,197; development) and PRIMUM (502; validation). German general practice trials. | Prognostic model development; assessment of anticholinergic burden scales and patient-reported symptoms. | No final prediction results in this protocol. Planned to evaluate the additional predictive value of anticholinergic symptoms for falls. | Yes (planned) |Falls are self-reported, with potential recall bias. Important predictors such as dementia, muscle strength, and gait problems could not be included. The external validation dataset has relatively few fall events. |
| 3 | Machado-Duque et al. (2024). Falls in hospitalized older adults and the use of fall risk-increasing drugs and anticholinergic medications in Colombia: A case-control study|10.3389/fphar.2024.1369200 | n = 1,250 (250 fall cases and 1,000 controls); four hospitals in Colombia (2018–2020) | Case-control study; conditional logistic regression | ARS score of 3 associated with increased fall probability: aOR = 2.34 (95% CI: 1.64–3.32). Polypharmacy and several FRID classes were also associated with falls. | No | Drug initiation dates, dosage, duration of prescriptions, laboratory data, and severity of clinical conditions were unavailable. |
| 4 | Gong et al. (2025). Patterns of Fall Risk-Increasing Drugs and Polypharmacy in Chinese Older Adults Before and After Fall-Related Fractures: A Single Center Retrospective Cohort Study. | 10.1177/30495334251385879 | n = 109; older adults with fall-related fractures at one hospital in China (2014–2019). | Retrospective cohort study; comparison of medication use before hospitalization, during hospitalization, and six months after discharge. | FRID use: 76.1% before hospitalization and 71.6% at six months. Polypharmacy: 59.6% and 57.8%, respectively. High-risk FRIDs decreased from 31.2% to 16.5% during hospitalization but recurrent prescribing reached 29.4% at follow-up. | No | Single-center study limits generalizability. OTC medications were not included, and medication exposure may change over longer follow-up periods. |
| 5 | Gagnon et al. (2026). Polypharmacy as a Simple Measure for Assessing the Risk of Fall-Related Hospitalization in Older Adults. | 10.1016/j.amepre.2025.108206 | n = 1,177,520; Quebec Integrated Chronic Disease Surveillance System, Canada (647,795 women and 529,725 men). | Population-based cohort study; sex-stratified Cox regression; comparison of five medication-based measures. | Highest predictive performance: ≥1 FRID, c-statistic = 0.735 (women), 0.736 (men). ≥1 PIM had the lowest performance: 0.724 and 0.722, respectively. | No | OTC medication data unavailable. The outcome only captures fall-related hospitalizations, not all falls. The hospitalization identification method was not based on a validated algorithm. |
| 6 | AlHarkan et al. (2023). Associations between polypharmacy and potentially inappropriate medications with risk of falls among the elderly in Saudi Arabia. | 10.1186/s12877-023-03852-y | n = 387; outpatient participants aged ≥60 from a university hospital and family/community medicine center in Khobar, Saudi Arabia (2021–2022). | Cross-sectional epidemiological study; patient interviews; multiple logistic regression; Beers Criteria for PIM identification. | 50.90% had polypharmacy; 51.42% were positive for Beers Criteria; 55% had high fall risk. Polypharmacy and PIMs were significantly associated with fall risk. | No | Fall history relied on patient recall; medication duration and drug-drug interactions were not considered. |
| 7 | Xue et al. (2021). Persistent polypharmacy and fall injury risk: the Health, Aging and Body Composition Study. | 10.1186/s12877-021-02695-9 | n = 1,764; Health ABC cohort linked with Medicare Fee-for-Service claims, USA. 545 incident fall injuries. | Prospective cohort analysis; time-varying Cox regression; sensitivity analyses involving FRID use. | Persistent polypharmacy associated with fall injury risk: HR = 1.31 (95% CI: 1.06–1.63). Persistent polypharmacy combined with FRID use was associated with a 48% higher risk compared with non-persistent polypharmacy without FRIDs. | No | Fall injuries rather than all falls were measured. FRID classification was adapted to the study context, and the selected cohort and Medicare-linked data may limit generalizability. |
| 8 | Wong et al. (2023). Polypharmacy and cumulative anticholinergic burden in older adults hospitalized with fall. | 10.1002/agm2.12250 | n = 411; acute medical admissions of older adults (≥65 years) at a UK district general hospital. | Prospective observational cohort study; electronic health records; multivariate analysis of polypharmacy and ACB. | Polypharmacy: OR = 2.14 (95% CI: 1.19–3.87). Each unit increase in ACB: OR = 1.15 (95% CI: 1.02–1.29). Both were significantly associated with falls. | No | Limited to a single hospital and a relatively small sample. Observational design cannot establish causality. |
| 9 | Ie et al. (2021). Fall Risk-Increasing Drugs, Polypharmacy, and Falls Among Low-Income Community-Dwelling Older Adults. | 10.1093/geroni/igab001 | n = 343; Falls Free PA program linked with Pennsylvania PACE prescription claims, USA. | Retrospective cohort study; negative binomial regression; comparison of six medication exposure measures. | ≥2 FRIDs independently predicted falls: adjusted IRR = 1.67 (95% CI: 1.04–2.68). Antidepressants were the only FRID class independently associated with increased falls. | No | OTC medications and medication adherence were not captured. Small sample size and low-income eligibility criteria limit generalizability. |
| 10 | van der Velde et al. (2023). European position paper on polypharmacy and fall-risk-increasing drugs recommendations in the World Guidelines for Falls Prevention and Management: implications and implementation. | 10.1007/s41999-023-00824-8 | N/A; European Geriatric Medicine Society (EuGMS) working group and World Guidelines recommendations. | Position paper; synthesis of clinical guidelines, research evidence, and expert recommendations. | Recommends structured medication review, FRID identification using tools such as STOPPFall, and appropriate deprescribing as part of multifactorial fall prevention. | N/A | Not an empirical validation study. Existing intervention studies have limitations related to suboptimal implementation of medication review and deprescribing. |

### A3. Research gaps
| ID | Gap (1–2 sentences) | Evidence (# in A2) | How your project addresses it |
|---|---|---|---|
| G1 | Incomplete medication-related risk assessment. Existing approaches often evaluate polypharmacy, FRIDs, or ACB separately. | 1;3;8 | There is an opportunity to integrate these dimensions with clinically significant drug-drug interactions. |
| G2 | Need for integrated predictive decision support. Existing studies demonstrate associations between medication-related factors and falls, but further research is needed to evaluate integrated machine learning prediction combined with rule-based DDI detection. | 2;7;9 | Integrate machine learning method with rule-based detection to develop a DDI detection component that provides better predictive performance than conventional statistical baselines. |

### A4. PROBAST+AI appraisal of the most important paper in A2
Paper #: 2 · Why this paper:
| Domain | Risk of bias (low / high / unclear) | Justification (quote or page number in the paper) |
|---|---|---|
| Participants and data sources | Unclear | Uses two cluster-randomized trials: RIME (n=1,197) for model development and PRIMUM (n=502) for external validation. However, participants were selected from German general practices, potentially limiting generalizability. (p. 1) |
| Predictors | Unclear | Candidate predictors were selected based on literature, predictor availability, and clinical reasoning. Five anticholinergic scales were considered: ADS, ARS, DBI, MARANTE, and Ger-ABS. However, some variables were unavailable in the validation dataset. (pp. 3–4) |
| Outcome | High | Falls were classified as no falls versus at least one fall within six months, based on patient interviews. The authors acknowledged possible recall bias and that falls could not be verified through electronic medical records. (pp. 1, 7) |
| Analysis | High | The planned model uses backward elimination based on AIC. Although bootstrap internal validation is planned, the authors acknowledge that the external validation dataset contains only 75 fall events, below the suggested minimum of 100 events. This could produce imprecise validation estimates. (pp. 6–8) |
Applicability to your team's problem: Provides a research framework for predicting fall risk in older adults by combining medication-related factors with individual patient characteristics.

## B. Results and timeline

### B1. Current results
| Model | Evaluation set (split method, n) | Main metric (value, 95% CI if available) | Secondary metrics | Source of numbers (file / notebook / W&B) |
|---|---|---|---|---|
| Baseline 1 (Milestone 2): Logistic Regression | 80/20 split test, 44 patients with 18,807 drug inscriptions | | | |

### B2. Ablation (Milestone 3)
| Configuration (component removed / changed) | Main metric | Difference vs full model | Source |
|---|---|---|---|

### B3. Comparison with the literature
Compare B1 with 2–3 papers from A2. State clearly anything that makes the comparison **unfair**: different dataset, different split, different metric.

### B4. Timeline to completion
| Task | Owner (student ID / role) | Milestone (M3 week 10 · M4 week 12 · Final week 15) | Planned date | Status (Not started / In progress / Done + evidence) |
| Complete literature review and verify at least 10 research papers | 202414856 | Week 3 | Week3 | Done |
| Complete data exploration and preprocessing | 202414831 | Week6 | Week6 | Done |
| Develop and evaluate baseline models | 202414856 / 202414831 | Week10 | Week10 | In progress |
| Complete proposed model and hyperparameter tuning | 202414856 / 202414831 | Week12 | Week12 | Not started |
| Conduct ablation experiments and model interpretation | 202414856 / 202414831 | Week14 | Week14 | Not started |
| Final evaluation, calibration and report preparation | 202414856 / 202414831 | Final – Week 15 | To be confirmed | Not started |
### B5. Risks / blockers / questions for the instructor
- The source and definition of high_fall_risk are not documented in the CSV
- The formula for fall_risk_score is not documented
- The ACB calculation method is not documented in the processed dataset
- The dataset contains only 100 patient records
- No verified model evaluation outputs are currently available
- No completed ablation results are available


## C. Self-assessment against the FAIR, TRIPOD+AI, PROBAST+AI appendix

### C1. FAIR — data
| Item | Answer | Evidence |
|---|---|---|
| Source, version, download date; checksum of the training file | Source: MIMIC-IV Clinical Database Demo. Consisting of 26 tables including age, drug prescriptions and comorbidity. Total of 100 demo patients. Download date, exact version and file checksum have not yet been documented. | |
| Licence / DUA; basis for being allowed to use the data | Dataset is restricted to educational purposes according to the current project report. The exact licence and applicable terms of use must be verified on the original dataset page. | |
| Datasheet: population, inclusion/exclusion criteria, variable definitions and units, limitations | | |
| No patient identifiers | | |

### C2. Reporting guideline
- Your research question: How do you integrate machine learning with rule-based hard stop component to design a system able to detect fall risk based on anticholinergic burden caused by drug-drug interaction from polypharmacy.
- Matching reporting guideline (TRIPOD+AI / STARD-AI / DECIDE-AI) and why (Appendix §3.2): TRIPOD+AI, our project develops and evaluates a machine learning-based prediction model using structured clinical and demographic data to calculate fall risk.
- Checklist items met / total; items still missing: Not yet fully assessed. A completed TRIPOD+AI checklist is required.
- Outcome, label, prediction time T0, variables available at T0: The dataset contains 5 labels: gender, anchor_age, drug, starttime, stoptime. Prediction time T0 is set at stoptime.

### C3. PROBAST+AI — self-appraisal of your project
| Domain | Risk of bias (low / high / unclear) | Evidence in the repo (file, line) | What you will do to reduce the risk |
|---|---|---|---|
| Participants and data sources | | | |
| Predictors | | | |
| Outcome (watch for incorporation bias) | | | |
| Analysis (patient-level split, fit on train only, sample size, missing data) | | | |
Applicability (population, setting where the model would be used):

### C4. Quick checklist (Appendix §7)
| Item | Met / Not yet | Evidence |
|---|---|---|
| Datasheet | Met | |
| Data version + checksum | Met | |
| No identifiers; basis for data use | Not met | |
| Correct reporting guideline + completed checklist | Not met | |
| Outcome, label, T0 defined | Met | |
| Patient-level split; preprocessing fit on train only | Met | |
| Logistic regression baseline (or a suitable baseline, with reason) | Not met | |
| AUC + calibration (curve, in-the-large, slope) + Brier, with 95% CI | Not met | |
| Is the sample size sufficient; applicability limits | Not met | |

## D. AI use declaration
| Tool | Used for which part | How the team verified the output |
|---|---|---|
| Claude | Drafting, organizing and condensing the project report based on the group's slides, research and notebook. | The group reviewed the generated content against the original slides, research papers and notebook results. |
| ChatGPT | Assistance with literature review, methodological appraisal. | Student must manually verify the entries suggested. |
