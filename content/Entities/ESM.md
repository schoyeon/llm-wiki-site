---
aliases: [ESM, ESM2, protein language model]
tags: [entity, tool, ML, protein]
sources: [The Virtual Lab_s41586-025-09442-9.pdf]
created: 2026-05-14
updated: 2026-05-14
---

# ESM (Evolutionary Scale Modeling)

Meta AI에서 개발한 protein language model. 단백질 서열의 evolutionary fitness를 평가.

## Key Points

- Amino acid sequence에 대한 log-likelihood를 계산하여 mutation의 영향 예측
- **LLR (Log-Likelihood Ratio)**: mutant vs wildtype의 likelihood 비교
- **ESM LLR^WT**: mutant sequence와 wildtype 간의 ratio — 높을수록 더 나은 mutation
- Virtual Lab에서 첫 번째 필터로 사용: single point mutation 제안 → top 20 선택

## Virtual Lab Pipeline에서의 역할

1. Input nanobody sequence에 대해 모든 single-point mutation의 LLR 계산
2. Top 20 mutant 선택
3. 이 20개를 [[AlphaFoldMultimer]]로 구조 예측

## Cross-References

- [[Swanson2025_VirtualLab|Virtual Lab 논문]]
- [[AlphaFoldMultimer]]
- [[Rosetta]]

## Source Citations
- [The Virtual Lab_s41586-025-09442-9.pdf]
