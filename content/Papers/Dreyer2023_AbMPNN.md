---
aliases: [AbMPNN paper]
tags: [paper, antibody, inverse-folding]
sources: [abmpnn_WCBICML2023_paper61.pdf]
created: 2026-05-14
updated: 2026-05-14
---

# Inverse folding for antibody sequence design using deep learning

**Authors:** Frédéric A. Dreyer, Daniel Cutting, Constantin Schneider, Henry Kenlay, Charlotte M. Deane
**Source:** ICML Workshop on Computational Biology (WCB), 2023

## Summary

AbMPNN은 ProteinMPNN을 항체에 특화시킨 inverse folding 모델이다. SAbDab (Structural Antibody Database)와 OAS (Observed Antibody Space)에서 fine-tuning하여 항체 구조에서의 서열 예측 성능을 향상. 특히 CDR-H3 루프 (antigen binding에 가장 중요한 영역)에서 현저한 개선을 달성.

## Key Points

- ProteinMPNN 아키텍처를 항체 데이터로 fine-tuning
- **CDR-H3** (가장 가변적이고 중요한 루프)에서 notable improvement
- Training data: SAbDab (3,500 complex) + OAS (147,919 paired sequences)
- Canonical CDR conformation의 improved encoding
- Drug discovery와 binder design에 응용 가능

## Cross-References

- [[Dauparas2022_ProteinMPNN|ProteinMPNN]] — 기반 모델
- [[Hoie2024_AntiFold|AntiFold]] — 유사한 antibody inverse folding
- [[Nanobody]]

## Source Citations
- [abmpnn_WCBICML2023_paper61.pdf]
