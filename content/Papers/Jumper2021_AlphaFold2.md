---
aliases: [AlphaFold 2 paper, AF2 paper]
tags: [paper, structure-prediction, deep-learning]
sources: [alphafold2_s41586-021-03819-2.pdf]
created: 2026-05-14
updated: 2026-05-14
---

# Highly accurate protein structure prediction with AlphaFold

**Authors:** John Jumper, Richard Evans, Alexander Pritzel, Tim Green, ..., Demis Hassabis
**Journal:** Nature, Vol 596, 2021
**DOI:** 10.1038/s41586-021-03819-2

## Summary

AlphaFold 2는 아미노산 서열로부터 단백질 3D 구조를 원자 수준 정확도로 예측하는 딥러닝 모델이다. CASP14에서 압도적 1위를 차지했으며, MSA와 structural template 정보를 Evoformer로 처리한 후 Structure module에서 3D 좌표를 생성한다. Backbone 정확도 0.96 Å (median), 전체 원자 정확도 1.5 Å을 달성.

## Key Points

- **Evoformer** (48 blocks): MSA representation + pair representation을 반복적으로 업데이트
- **Structure module** (8 blocks): Invariant Point Attention (IPA)으로 equivariant 3D 좌표 생성
- **Recycling**: 전체 네트워크를 3회 반복하여 정확도 향상
- **pLDDT**: per-residue confidence score — Ca LDDT를 직접 예측
- **CASP14**: median backbone accuracy 0.96 Å (2위: 2.8 Å)
- 후속 모델: [[AlphaFoldMultimer]], [[AlphaFold3]]

## Cross-References

- [[Abramson2024_AlphaFold3|AF3 논문]] — 후속 모델
- [[AlphaFoldMultimer]] — complex 예측 확장
- [[AlphaFold3]]
- [[StructurePrediction]]
- [[DemisHassabis]]
- [[JohnJumper]]

## Source Citations
- [alphafold2_s41586-021-03819-2.pdf]
