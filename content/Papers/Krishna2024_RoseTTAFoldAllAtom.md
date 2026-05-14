---
aliases: [RFAA paper, RoseTTAFold All-Atom paper]
tags: [paper, structure-prediction, protein-design]
sources: [rf2-aa_science.adl2528.pdf]
created: 2026-05-14
updated: 2026-05-14
---

# Generalized biomolecular modeling and design with RoseTTAFold All-Atom

**Authors:** Rohith Krishna, Jue Wang, Woody Ahern, Pascal Sturmfels, ..., David Baker
**Journal:** Science, Vol 384, 2024
**DOI:** 10.1126/science.adl2528

## Summary

RFAA (RoseTTAFold All-Atom)는 단백질뿐 아니라 핵산, 소분자, 금속 이온, 공유 변형까지 포함하는 범용 생체분자 구조 예측 및 설계 모델이다. RF2 아키텍처를 확장하여 소분자를 atom-bond graph로, 핵산을 화학 원소 단위로 표현. RFdiffusionAA로 확장하여 소분자 결합 단백질 de novo 설계도 가능. 심장 약물 digoxigenin 등에 대한 binder 설계를 실험적으로 검증.

## Key Points

- **입력 범위**: 단백질 + DNA/RNA + 소분자 + 금속 이온 + 공유 변형 (인산화 등)
- RF2의 3-track에 소분자용 atom-bond graph track 추가
- **RFdiffusionAA**: RFAA 기반 de novo 소분자 binder 설계
- CAMEO blind ligand-docking challenge에서 baseline 대비 우수
- [[AlphaFold3]]와 유사한 범용성이지만, 오픈소스

## Cross-References

- [[Baek2023_RoseTTAFold2|RF2 논문]] — 기반 모델
- [[Abramson2024_AlphaFold3|AF3 논문]] — 유사한 범용 모델
- [[Watson2023_RFdiffusion|RFdiffusion]] — 단백질 설계
- [[StructurePrediction]]
- [[DiffusionModel]]

## Source Citations
- [rf2-aa_science.adl2528.pdf]
