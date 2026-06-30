# Praxis — Supplementary Materials

Reproducibility archive for the doctoral praxis:

**The Impact of Project Management and Risk Management on EdTech Implementation
Success in Higher Education Institutions: A Path Analysis and Risk Prioritization
Approach** — Rajni Ekta Soharu, The George Washington University, School of
Engineering and Applied Science (D.Eng.).

Repository: https://github.com/rsoharu/Praxis

---

## Overview

This repository hosts the supplementary materials referenced in Appendices A and B
of the praxis. The study analyzes an archival dataset of 197 completed EdTech
projects, specifying three reflective constructs — Project Management (PM), Risk
Management (RM), and Implementation Success (IS) — and estimating a composite-based
structural path model. It introduces the Adjusted Risk Score (ARS = P × I × β) and
the EdTech Implementation Risk Intelligence System (EIRIS) for risk prioritization.

## Contents

| Folder | Contents |
|--------|----------|
| `code/` | Python (pandas) analysis pipeline: composite construction, standardized OLS path estimation, 5,000-sample BCa bootstrap, and ARS computation. |
| `data/` | De-identified scored indicator matrix for the 197 projects. |
| `amos/` | Full IBM SPSS AMOS CB-SEM measurement-model output (Appendix A). |
| `bootstrap/` | Bootstrap sampling distributions for the indirect effect (Appendix B). |
| `eiris/` | The EIRIS Adjusted Risk Score (ARS) spreadsheet tool. |

## Key reported results

- **RM → IS**  β = 0.380 (t = 5.721, p < .001)
- **PM → IS**  β = 0.143 (t = 2.151, p = .033)
- **PM → RM**  β = 0.227 (p = .001)
- **Indirect (PM → RM → IS)**  β = 0.0848, 95% BCa CI [0.0287, 0.1484] (partial mediation)
- **Total PM effect**  0.229
- **R² (IS)**  0.189
- **ARS tiers**  0 Critical · 25 High · 105 Moderate · 67 Low

## Reproduce

```bash
python -m pip install pandas numpy scipy
python code/eiris_research.py
```

## Citation

> Soharu, R. E. (2026). *Praxis — Supplementary Materials* [Data set and code].
> GitHub. https://github.com/rsoharu/Praxis

## License

- Code: MIT
- Data and figures: CC BY 4.0

---

*Before publishing the dataset, confirm that all institution names, project
identifiers, and personnel have been removed; publish only the nine indicator
scores and the derived composites used in the analysis.*
