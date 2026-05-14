---
aliases: [AF3, AlphaFold 3, AlphaFold3]
tags: [entity, tool, structure-prediction, deep-learning]
sources: [alphafold3_s41586-024-07487-w.pdf]
created: 2026-05-14
updated: 2026-05-14
---

# AlphaFold 3

Google DeepMind에서 개발한 범용 생체분자 구조 예측 모델. 단백질, DNA, RNA, 리간드, 이온, 공유 변형 잔기를 포함한 복합체 구조를 통합 예측.

## Key Points

- [[AlphaFoldMultimer]] (AF-M 2.3)의 후속 모델
- **Diffusion 기반**: Structure module 대신 diffusion module로 원자 좌표 직접 예측
- **Pairformer**: Evoformer를 간소화한 pair-representation 중심 아키텍처
- **범용성**: protein-only가 아닌 모든 생체분자 복합체 예측 가능
- **AlphaFold Server** (alphafoldserver.com)에서 무료 사용

## AF2/AF-M 2.3 vs AF3

| 특징 | AF-M 2.3 | AF3 |
|------|----------|-----|
| MSA 처리 | Evoformer (48 blocks) | Pairformer (MSA 4 blocks만) |
| 구조 예측 | Structure module (equivariant) | Diffusion module |
| 입력 범위 | 단백질 복합체 | 단백질+DNA+RNA+리간드+이온 |
| 항체-항원 | 보통 | 대폭 향상 |
| Confidence | pLDDT, pTM, PAE | pLDDT, pTM, ipTM, PAE, DockQ |

## Virtual Lab 파이프라인과의 관계

[[Swanson2025_VirtualLab|Virtual Lab]]에서는 [[AlphaFoldMultimer]] (AF-M 2.3)를 사용하여 nanobody-spike 구조를 예측했다. AF3가 출시되었지만, Virtual Lab 연구 시점에는 AF-M이 사용됨. AF3는 antibody-antigen 예측이 크게 개선되어, 향후 nanobody 설계에 AF3 적용 시 더 나은 결과가 기대됨.

## Cross-References

- [[Abramson2024_AlphaFold3|AF3 논문]]
- [[AlphaFoldMultimer]] — 전신
- [[DiffusionModel]] — 핵심 아키텍처
- [[StructurePrediction]] — 상위 개념
- [[DemisHassabis]]
- [[JohnJumper]]

## Source Citations
- [alphafold3_s41586-024-07487-w.pdf]
