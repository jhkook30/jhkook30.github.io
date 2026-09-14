---
title: "Efficiency Evaluation of Sparsified Homomorphic Encryption in Federated Learning"
collection: publications
category: conferences
permalink: /publication/2025-11-sparsified-he-fl
excerpt: 'We measured what homomorphic encryption actually costs in federated learning, and how much of that cost sparsification can recover. On MNIST, Top-k sparsification cut communication by 4.3x and training time by 1.6x, at the price of 1.2%p accuracy.'
date: 2025-11-21
venue: 'Korean Institute of Communications and Information Sciences (KICS) Fall Conference'
slidesurl: # '/files/slides-kics2025.pdf'
paperurl: 'https://www.dbpia.co.kr/journal/articleDetail?nodeId=NODE12567025'
bibtexurl: # '/files/bibtex_kics2025.bib'
citation: '<b>Jihyung Kook</b>, Eunsang Lee (2025). &quot;Efficiency Evaluation of Sparsified Homomorphic Encryption in Federated Learning.&quot; <i>Proceedings of the KICS Fall Conference</i>, pp. 752-753.'
---

<span style="color:#666">
요약: 연합학습에 동형암호를 적용하면 프라이버시는 강해지지만 통신량과 연산량이 함께 늘어납니다. 이 포스터에서는 그 비용을 MNIST 기준으로 정량화하고, 희소화(Top-k)로 얼마나 회복할 수 있는지 측정했습니다. 평문 대비 동형암호는 통신량이 13.2배 늘었는데, 희소화를 적용하자 그 중 상당 부분이 되돌아왔습니다. 정확도 손실은 1.2%p 수준이었습니다.
</span>

### ⚡️ TL;DR
Homomorphic encryption makes federated learning private but expensive. We measured how expensive, and found that **Top-k sparsification recovers most of the communication cost** with a small accuracy loss.

### 👩🏻‍💻 My Role
- Designed and ran all three experimental conditions under a unified setup.
- Implemented the CKKS-based pipeline and the Top-k sparsification path.
- Analyzed results and wrote the paper.

### 🧪 Methods / Data
- **Dataset:** MNIST, evenly distributed across 10 clients.
- **Conditions:** (i) plaintext FL, (ii) CKKS-based HE-FL, (iii) HE-FL with Top-k sparsification (20%).
- **Setup:** up to 100 epochs, early stopping when accuracy improved less than 0.1%p for 10 consecutive epochs.
- **Metrics:** accuracy, training time, network traffic, and rounds to convergence.

### 📊 Results / Impact

| Metric | Plain-FL | HE-FL | HE-Spars-FL |
|---|---|---|---|
| Accuracy (%) | 98.9 | 95.1 | 93.9 |
| Training time (s) | 75.7 | 214.1 | 133.0 |
| Communication (MB) | 166 | 2,198 | 512 |
| Rounds to converge | 39 | 35 | 26 |

- Encryption cost **2.8x training time** and **13.2x communication** over plaintext.
- Sparsification brought communication down **4.3x** (2,198 → 512MB) and training time down **1.6x** (214.1 → 133.0s).
- Accuracy dropped only **1.2%p** against HE-FL, so the efficiency gain does not come at a meaningful cost in utility.
- This gap — the distance between a private system and a deployable one — is what my current work on sparsification-friendly CKKS aims to close.