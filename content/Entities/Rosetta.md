---
aliases: [Rosetta, RosettaScripts]
tags: [entity, tool, computational-biology]
sources: [The Virtual Lab_s41586-025-09442-9.pdf]
created: 2026-05-14
updated: 2026-05-14
---

# Rosetta

단백질 구조 모델링 및 에너지 계산 소프트웨어. David Baker 그룹(UW) 개발.

## Key Points

- **RS dG (separated dG)**: complex에서 각 chain을 분리했을 때의 에너지 변화 — binding energy의 proxy
- 더 음수(negative)일수록 더 강한 binding
- Virtual Lab에서는 [[AlphaFoldMultimer]] 예측 구조를 relaxation한 후 dG 계산

## Virtual Lab Pipeline에서의 역할

1. AF-Multimer 예측 구조에 Rosetta relaxation 적용
2. Separated dG (RS dG) 계산
3. 최종 Weighted Score에 반영: WS = 0.2 × ESM LLR + 0.5 × AF ipLDDT − 0.3 × RS dG

## Cross-References

- [[Swanson2025_VirtualLab|Virtual Lab 논문]]
- [[ESM]]
- [[AlphaFoldMultimer]]

## Source Citations
- [The Virtual Lab_s41586-025-09442-9.pdf]
