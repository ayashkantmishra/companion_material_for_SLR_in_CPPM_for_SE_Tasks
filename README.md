# Companion Files for the SLR on Cross-Project Predictive Modelling for Software Engineering Tasks

This repository contains the companion files for the systematic literature review on cross-project predictive modelling in software engineering. The material is provided to make the search, screening, rejection, and final study-selection process transparent and easier to verify.

The review focuses on cross-project prediction studies in software engineering published between 2015 and 2025. The scope is broader than cross-project defect prediction alone and includes software engineering prediction tasks such as defect prediction, vulnerability detection, just-in-time defect prediction, effort estimation, bug localization, self-admitted technical debt detection, and other related cross-project prediction settings.

---

## Repository Contents

```
.
├── README.md
├── Paper_Selection_Excel.xlsx
├── Companion Material.pdf
└── bibliography.bib
```

---

## Files

### 1. `Supplementary_Paper_Selection.xlsx`

This Excel file contains the complete paper-screening record used in the review. It is organized into four sheets:

| Sheet name | Description |
|---|---|
| All Studies(After Preprocessing) | Contains all papers retained after initial preprocessing and duplicate removal. |
| Pass1_Rejections | Contains papers rejected during the first screening stage. |
| Pass2_Rejections | Contains papers rejected during the second screening stage. |
| Selected_Studies_132 | Contains the final 132 primary studies selected for the review. |

The Excel file is intended to help reviewers inspect how the final set of selected studies was obtained from the larger candidate set.

### 2. `Search_Strings_and_Selected_Studies_Appendix.pdf`

This PDF contains the supplementary appendix for the review. It includes:

- the final search string used in the review;
- the iterative search strings used during query refinement;
- the list of selected primary studies;
- the appendix version of the selected-paper table.

The PDF is provided for easy reading and citation alongside the manuscript.

### 3. `bibliography.bib`

This BibTeX file contains the bibliographic records used in the review and supplementary appendix of the selected studies. The citation keys used in the appendix correspond to this BibTeX file.

---

## Study-Selection Criteria

### Inclusion Criteria

A paper was included if it satisfied all of the following conditions:

- The paper was published between 2015 and 2025.
- The paper addressed a cross-project prediction problem in a software engineering context.
- The paper used or reported datasets that are publicly available or reproducible from public sources.
- The paper was at least four pages long.
- The paper was a peer-reviewed research article, conference paper, journal paper, or workshop paper with sufficient methodological content.
- The paper contained enough information to support extraction for the review questions.

### Exclusion Criteria

A paper was excluded if it met any of the following conditions:

- The paper addressed only within-project prediction and did not include a cross-project setting.
- The paper was outside the software engineering prediction context.
- The paper did not use publicly available or reproducible datasets.
- The paper was a tutorial, keynote, editorial, short abstract, poster summary, discussion article, or non-primary-study material.
- The paper was less than four pages long.
- The paper was a duplicate or near-duplicate of another record already retained in the candidate set.
- The paper did not provide enough methodological or experimental detail for reliable extraction.

---

## Screening Process

The screening process was conducted in two main passes after initial preprocessing.

### Initial Preprocessing

In this stage, records collected from the selected digital libraries were cleaned before detailed screening. Preprocessing included:

- removing duplicate records;
- checking publication year;
- checking publication type;
- removing clearly irrelevant records;
- standardizing available bibliographic information such as title, year, venue, DOI, and publisher.

The cleaned candidate set is reported in the sheet **All Studies(After Preprocessing)**.

### Pass 1 Screening

Pass 1 was a broad eligibility screening based mainly on title, keywords, metadata, and basic publication information.

A paper could be rejected in Pass 1 for reasons such as:

- outside the 2015--2025 time window;
- not related to software engineering prediction;
- no visible cross-project component from the title, keywords, or metadata;
- non-research publication type;
- duplicate record;
- insufficient length;
- tutorial, keynote, editorial, abstract-only, or discussion material.

The records rejected at this stage are listed in the sheet **Pass1_Rejections**.

### Pass 2 Screening

Pass 2 involved a closer inspection of the abstract and, when necessary, the full text.

A paper could be rejected in Pass 2 for reasons such as:

- the study used only within-project prediction;
- the cross-project component was mentioned but not actually evaluated;
- the dataset was not publicly available or reproducible;
- the study was not focused on a software engineering prediction task;
- the paper did not provide sufficient methodological or experimental detail;
- the paper was a secondary study, survey, or review rather than a primary empirical study;
- the paper did not align with the review questions.

The records rejected at this stage are listed in the sheet **Pass2_Rejections**.

### Final Selected Studies

After Pass 1 and Pass 2 screening, 132 primary studies were selected for the final review. These studies are listed in the sheet **Selected_Studies_132**.

The selected studies form the basis for answering the review questions related to:

- software engineering prediction tasks;
- software artifacts used for prediction;
- datasets and benchmark families;
- heterogeneity-handling methods;
- machine learning and deep learning models;
- evaluation metrics;
- statistical tests and validation practices.
