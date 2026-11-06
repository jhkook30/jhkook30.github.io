---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

[Download CV (PDF)]({{ '/files/CV%20-%2020261107.pdf' | relative_url }}) · Updated November 7, 2026

## Research interests
Verifiable and privacy-preserving computation; applied cryptography (zero-knowledge proofs, homomorphic encryption, and multi-party computation); AI security and privacy.

## Education
- **Georgia Institute of Technology** — Online M.S. in Computer Science, December 2024. Specialization: Computational Perception & Robotics.
- **Sookmyung Women's University** — B.S. in Statistics and Computer Science, February 2017.

## Manuscripts

- **Kook, J.**, Kang, D., and Lee, E. *Sparsification-Friendly CKKS-Based Federated Learning via RLWE-to-MLWE Conversion.* **In preparation.**
- Yoo, S., Oh, T., **Kook, J.**, et al. *Association between Muscle Cramping and Diabetic Peripheral Neuropathy: Findings from a Prospective Cohort Study.* **Under review**, Diabetes & Metabolism Journal, June 2026.

## Publications and presentations
<ul>{% for post in site.publications reversed %}
  {% include archive-single-cv.html %}
{% endfor %}</ul>

## Research experience

### Independent research: Adversarial analysis of verifiable model certification
**Co-organizer, Georgia Tech OMSCS ZKP Study Group · August 2026–present**

- Analyze fixed-point tolerance constraints in FairProof's Go/gnark implementation and adapt existing circuits to test malicious witnesses that inflate claimed distances while satisfying the constraints.
- Constructed a synthetic ReLU-network proof of concept with a reported fairness radius of 0.8775 versus 0.0277 (31.6×), with all 24 logged component checks passing under locally configured tolerances.
- Reproduced collaborator-provided output-layer scaling experiments on the supplied model, observing up to 14.7% radius inflation relative to honest runs with all 776 Groth16 verification checks passing.
- Prepare further experiments on deeper networks and study FairZK.

### Sejong University: Privacy-Preserving Machine Learning and Cryptography Lab
**Full-time Researcher · July 2025–present**<br />
Advisor: [Prof. Eunsang Lee](https://sites.google.com/view/pmlclab/home)

- Lead experimental design for threshold-CKKS federated learning, screening chunk sizes and selection ratios in plaintext before evaluating CIFAR-10/100 configurations using OpenFHE/C++ across three seeds.
- Achieved 89% accuracy on CIFAR-10 and 65% on CIFAR-100 at B = 1 and ρ = 0.1, with 1.3–1.6× online communication ratios and 1.7–25.9% higher estimated parallel runtime relative to plaintext baselines.
- Reduced cumulative online communication by 66–67% across CIFAR-10 and CIFAR-100 through sparse aggregation (ρ = 0.3, B = 512), with accuracy decreases of less than one percentage point compared with full encrypted aggregation.

### Independent research: Privacy leakage in agentic AI
**Research Collaborator · July–September 2026**

- Developed three- and four-layer MLP classifiers on 3,190 simulated healthcare-agent traces to infer sensitive patient attributes from tool names alone.
- Compared bag-of-tools frequency features with chronological n-gram features across three prediction tasks; achieved a macro-F1 of 0.689 for treatment complexity without invocation-order information.

### Seoul National University Bundang Hospital
**Part-time Researcher, Endocrinology & Metabolism · March 2018–July 2020**<br />
Advisor: Prof. Tae Jung Oh

- Managed clinical data for a retrospective study of a standardized glucose-insulin-potassium infusion protocol.
- Conducted 1:1 propensity score matching (227 patients per group), blood-glucose interpolation, and comparisons of glucose AUC and time within the target range in R.
- Engineered features from continuous glucose monitoring data from 55 patients; achieved an AUC of up to 0.88 with support vector classification using peak-timing and glucose-variability measures.

## Professional experience

### Seoul National University Bundang Hospital
**Part-time Research Assistant, Endocrinology & Metabolism · July 2025–present**

- Preprocess, merge, and analyze EMR datasets in Python; generate descriptive and sex-stratified tables and univariable logistic regression results for clinical manuscripts.
- Coordinate administration and support site preparation for a KDCA-funded multicenter pragmatic randomized trial of personalized risk score-based management for older adults with type II diabetes.

### KB Kookmin Bank & KB Financial Group
**Data Analyst, Department of Data Planning · July 2020–September 2023**

- Standardized customer data across seven subsidiaries into eight domains and implemented retention and deletion rules for a group-wide database.
- Coordinated quality reviews supporting cleanup of 20% of legacy records and updates to 10% of high-value datasets.
- Managed customer journey mapping and delivered SQL, Tableau, and automation training across seven subsidiaries, updating more than 30 topics annually.

### Croquis Inc. (now Kakao Style)
**Junior Data Analyst, Department of Data · March 2018–April 2020**

- Automated 17 ETL workflows with Python, PySpark, and SQL, improving data accuracy and reliability by 25%.
- Designed and evaluated A/B tests for a new-arrivals feed and developed a seller clustering model.
- Defined payment KPIs, built Tableau/R dashboards, and automated promotion reports. Early-adopting sellers recorded monthly sales 1.5× their pre-adoption levels.
- Delivered SQL and Tableau training, reducing the data team's workload by 10%.

## Additional training
**Seoul National University Big Data Institute · July 2017–February 2018**<br />
4th Industrial Revolution Academy: Big Data Platform Technology

- Completed intensive training in Python, SQL/DBMS, distributed systems, data mining, and machine/deep learning.
- Conducted an exploratory study at SNUBH on predictive factors in continuous glucose monitoring data.

## Skills
- **Programming:** Python, C/C++, Go, SQL, R, PyTorch, PySpark.
- **Cryptography, privacy, and systems:** CKKS, OpenFHE, federated learning, zero-knowledge proofs (gnark), Git, Docker, Linux.
- **Data analysis and research tools:** Statistical modeling, Matplotlib, ggplot2, Shiny, Tableau, LaTeX.
