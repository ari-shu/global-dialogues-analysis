# AI Governance and Institutional Intermediaries: Preliminary EDA on Global Dialogues GD3

Preliminary exploratory analysis of the Global Dialogues GD3 dataset, supporting a larger research project on the alignment between public AI governance preferences and national regulatory frameworks, with particular attention to institutional intermediaries (employers, schools, healthcare providers, public-sector agencies).

## Data

Data comes from CIP's public [`collect-intel/global-dialogues`](https://github.com/collect-intel/global-dialogues) repository. This analysis uses GD3 (March 2025).

Files used:
- `GD3_aggregate_standardized.csv`
- `GD3_participants.csv`
- `GD3_verbatim_map.csv`

## Setup

Python 3.10+. Install dependencies:

```bash
pip install pandas numpy jupyter
```

Run the notebook:

```bash
jupyter notebook global_dialogues_eda.ipynb
```

## Analysis

The notebook (a) identifies questions and responses related to institutional trust and governance through keyword filtering, (b) extracts the structured trust battery covering eight institutional categories, (c) filters to a target jurisdiction set (US, UK, India, China, Brazil), and (d) scans open-ended responses for organic mentions of workplaces, schools, and healthcare institutions.

## Preliminary findings

### Structured trust battery

GD3 contains eight purpose-built trust items measuring respondent trust in governments, large corporations, small businesses, social media companies, AI companies, public utility companies, public research institutions, and family doctors, each on a six-point ordinal scale (Strongly Distrust through Strongly Trust). The inclusion of AI companies as a distinct category, separable from large corporations and from public research institutions, supports decomposition of AI-specific distrust from baseline corporate or institutional distrust.

### Organic intermediary mentions in open-ended responses

Across the 360 respondents from the five target jurisdictions in GD3, open-ended responses to "What has been the most noticeable change in your daily life, if any, as a result of AI in the past year?" mention:

- Workplaces or employers in 6.1% of responses (22 of 360)
- Schools or education in 3.1% of responses (11 of 360)
- Healthcare institutions in 1.7% of responses (6 of 360)

Identification used keyword-lexicon filtering against eight workplace terms, seven education terms, and seven healthcare terms (see notebook for full lexicons). Sample responses are reproduced in the notebook output.

### Sample volumes by target jurisdiction (GD3)

| Country | N |
|---|---|
| India | 183 |
| China | 70 |
| United States | 52 |
| Brazil | 30 |
| United Kingdom | 25 |

## Limitations

Keyword-lexicon filtering produces false positives (a response mentioning "company" in passing) and false negatives (a response describing an institutional context without naming it). Single-round single-jurisdiction sample sizes are small; pooling across GD rounds will be necessary for stable cross-country estimates. Categorizations are provisional pending validation against embedding-based clustering and a human-coded sample.

## Next steps

- Validate keyword filtering against embedding-based clustering and a human-coded sample.
- Extend the analysis to GD4 through GD7.
- Run ordinal multilevel models on the structured trust battery items, decomposing trust in AI companies relative to corporate and institutional baselines.
- Integrate with comparative coding of national AI regulatory regimes.
