---
aliases: [structure prediction, protein structure prediction, 구조 예측]
tags: [concept, computational-biology, structural-biology]
sources: [alphafold3_s41586-024-07487-w.pdf]
created: 2026-05-14
updated: 2026-05-14
---

# Structure Prediction

아미노산 서열 등의 1D 정보로부터 3D 생체분자 구조를 예측하는 분야.

## Key Points

- 전통 방식: 물리 기반 시뮬레이션 (MD, Monte Carlo)
- 현대 방식: 딥러닝 기반 (AlphaFold 시리즈, RoseTTAFold 등)
- 핵심 평가 지표: LDDT, TM-score, GDT, RMSD, DockQ

## 주요 도구 계보

| 세대 | 도구 | 특징 |
|------|------|------|
| 1세대 | [[Rosetta]] | Physics-based energy function |
| 2세대 | AlphaFold 2 / [[AlphaFoldMultimer]] | Evoformer + Structure module |
| 3세대 | [[AlphaFold3]] | Pairformer + [[DiffusionModel]] |
| 병렬 | RoseTTAFold, ESMFold | 대안적 아키텍처 |

## Confidence Metrics

| Metric | 범위 | 의미 |
|--------|------|------|
| pLDDT | 0-100 | 잔기별 신뢰도. >90 매우 좋음, >70 좋음 |
| pTM / ipTM | 0-1 | 전체/interface 구조 품질 |
| PAE | Å | 잔기 쌍 간 예측 오차 |
| DockQ | 0-1 | >0.23 correct, >0.8 very high |
| iPAE | Å | interface 잔기의 PAE (낮을수록 좋음) |

## Cross-References

- [[Abramson2024_AlphaFold3|AF3 논문]]
- [[AlphaFold3]]
- [[AlphaFoldMultimer]]
- [[Rosetta]]
- [[DiffusionModel]]

## Source Citations
- [alphafold3_s41586-024-07487-w.pdf]
