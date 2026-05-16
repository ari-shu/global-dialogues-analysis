# AI Governance and Institutional Intermediaries: Analyzing Congruence in Collective Intelligence

An empirical research project investigating the alignment between public AI governance preferences and national regulatory frameworks, with a specific focus on the role of institutional intermediaries (employers, educational institutions, healthcare providers, and local public-sector agencies).

---

## Project Overview

Existing analyses of AI regulation tend to treat governance as a binary relationship between nation-states and AI developers, treating the public merely as an aggregated preference input. This framework overlooks the critical layer where AI governance is actually experienced by most people: institutional intermediaries that translate provider behavior and state regulations into daily workflows and interfaces.

This project introduces an intermediary-aware model of "democratic congruence" to investigate two core dimensions:
1. **Vertical Congruence:** Whether state-level regulatory outputs match public preferences across core dimensions (transparency, redress, deployment restrictions, public participation, and provider constraints).
2. **Architectural Congruence:** Whether the distribution of governance authority delegated to intermediaries matches the institutional trust allocations actually held by the public.

---

## Research Questions

1. **Regulatory Alignment:** Where do public preferences, as expressed across Global Dialogues rounds, converge or diverge from existing regulatory architectures across a comparative set of jurisdictions (US, UK, EU, China, India, Brazil)?
2. **The Architectural Choice:** Do publics in jurisdictions that delegate governance to intermediaries express trust commensurate with that delegated authority? Conversely, do centralized regimes reflect organic public demand for state intervention, or do they indicate institutional vulnerabilities?
3. **The Intermediary Gap:** Where governance architectures and trust allocations diverge, what are the implications for institutional design? (e.g., Are states empowering intermediaries that the public deeply distrusts, or failing to empower intermediaries that the public trusts?)

---

## Methodology and Analytical Stack

This work combines comparative legal coding, quantitative survey analysis, and computational text mining:

* **Structured Regulatory Coding:** Constructing a comparative dataset of 8–12 national regulatory regimes (including the EU AI Act, US Executive Orders, China’s Generative AI Rules, and Brazil's PL 2338) evaluated against structural dimensions derived from Global Dialogues indicators. Iterative Inter-Rater Reliability (IRR) protocols discipline the schema.
* **Quantitative Preference Analysis:** Multilevel modeling nesting individual respondents within countries, incorporating country-level covariates from the V-Dem Institute, OECD Trust Survey, and the Edelman Trust Barometer to isolate AI-specific dynamics from baseline institutional trust. 
* **Computational Text Mining:** Embedding-based clustering paired with keyword-lexicon string filtering to identify and categorize how respondents organically invoke intermediary layers when reasoning about AI.
* **Benchmarking and Representativeness:** Comparative analysis against the World Values Survey and regional Barometers, reporting diagnostics using the open-source Global Representativeness Index (GRI) framework (1 - TVD).

---

## Initial EDA and Empirical Signals (Wave: GD3)

An initial exploratory data analysis (EDA) conducted on the standardized GD3 (March 2025) dataset validated the empirical visibility of the intermediary layer within public reasoning:

### 1. Organic Intermediary Mentions
Parsing open-ended responses from the core target jurisdictions (US, UK, India, China, Brazil) surfaced significant, spontaneous discussion of downstream institutional mediation:
* **Workplace / Employers (~6.1% of target respondents):** Participants frequently frame AI's societal impact entirely through its deployment by their employers (e.g., "Help me with my job").
* **Education / Schools (~3.1% of target respondents):** Highlights critical institutional breakdown and friction points where schools fail to scaffold technology (e.g., students "blatantly using AI to finish assignments" resulting in "less intellectual growth").
* **Healthcare (~1.7% of target respondents):** Professional and clinical instances of intermediaries utilizing generative tools to scale domain-specific content production.

### 2. Available Target Sample Volume (N)
The underlying participant distributions offer robust analytical leverage for cross-country modeling:
* **India:** N = 183
* **China:** N = 70
* **United States:** N = 52
* **Brazil:** N = 30
* **United Kingdom:** N = 25

---

## Deliverables and Target Audience

* **Working Paper:** Full academic manuscript containing the multilevel model specifications, coding schema, and policy conclusions.
* **Substack Series:** A 3-part translational writing series covering:
  1. Headline empirical findings on state-level congruence.
  2. Deep dive into specific jurisdictions where the intermediary layer drives the trust gap.
  3. Actionable policy implications for institutional design.
* **Interactive Visualization:** A comparative country-dashboard mapping state delegation vs. public trust allocations.

**Primary Audiences:** UK and US Artificial Intelligence Safety Institutes (AISIs), the International Network of AI Safety Institutes, the Independent AI Evaluators Forum, and the EU AI Office.
