---
aliases: [AlphaFold-Multimer, AF-Multimer, AFM]
tags: [entity, tool, structure-prediction]
sources: [The Virtual Lab_s41586-025-09442-9.pdf]
created: 2026-05-14
updated: 2026-05-14
---

# AlphaFold-Multimer

DeepMind의 AlphaFold를 protein complex 예측으로 확장한 모델. Nanobody-antigen complex의 구조를 예측.

## Key Points

- **ipLDDT (interface pLDDT)**: 결합 interface 잔기들의 predicted LDDT 평균
- Interface 잔기 = 상대 chain의 잔기와 4Å 이내에 있는 잔기
- ipLDDT가 높을수록 interface 구조 예측 신뢰도가 높음 → 좋은 binding을 시사

## Virtual Lab Pipeline에서의 역할

1. [[ESM]]에서 선택된 top 20 mutant에 대해 nanobody-spike complex 구조 예측
2. ipLDDT 계산
3. 결과를 [[Rosetta]]의 dG 계산에 input으로 제공

## 후속 모델: AlphaFold 3

[[AlphaFold3]]가 AF-M 2.3을 대체. Evoformer → Pairformer, Structure module → [[DiffusionModel]]로 아키텍처 전환. 특히 antibody-antigen 예측 성능이 크게 개선됨.

## Cross-References

- [[Swanson2025_VirtualLab|Virtual Lab 논문]]
- [[Abramson2024_AlphaFold3|AF3 논문]]
- [[AlphaFold3]] — 후속 모델
- [[ESM]]
- [[Rosetta]]

## Source Citations
- [The Virtual Lab_s41586-025-09442-9.pdf]
- [alphafold3_s41586-024-07487-w.pdf]
