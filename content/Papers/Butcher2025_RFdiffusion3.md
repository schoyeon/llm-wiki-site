---
aliases: [RFdiffusion3 paper, RFD3]
tags: [paper, protein-design, diffusion, all-atom]
sources: [rfdiffusion3_2025.09.18.676967v2.full.pdf]
created: 2026-05-14
updated: 2026-05-14
---

# De novo Design of All-atom Biomolecular Interactions with RFdiffusion3

**Authors:** Jasper Butcher, Rohith Krishna, Raktim Mitra, Rafael I. Brent, ..., Frank DiMaio, David Baker
**Source:** bioRxiv, 2025
**DOI:** 10.1101/2025.09.18.676967

## Summary

RFdiffusion3 (RFD3)는 리간드, 핵산 등 비단백질 분자와의 상호작용을 포함하여 all-atom 수준에서 단백질 구조를 생성하는 diffusion 모델이다. 모든 polymer atom을 명시적으로 모델링하며, 복잡한 atom-level constraint 조건 하에서 설계 가능. 기존 방법 대비 1/10의 computational cost로 더 나은 성능. DNA-binding 단백질과 cysteine hydrolase를 설계·실험 검증.

## Key Points

- **All-atom diffusion**: backbone + sidechain + non-protein atom 전부 diffusion
- AF3의 diffusion module과 유사한 transformer-based U-Net 아키텍처
- 리간드, 핵산, 금속 이온 등 비단백질 분자 컨텍스트에서 설계
- 기존 RFdiffusion/RFdiffusion2 대비 더 범용적
- AtomWorks framework (RosettaCommons) 기반

## Cross-References

- [[Watson2023_RFdiffusion|RFdiffusion]] — 1세대
- [[Ahern2025_RFdiffusion2|RFdiffusion2]] — 2세대
- [[DiffusionModel]]
- [[AlphaFold3]] — 유사 아키텍처

## Source Citations
- [rfdiffusion3_2025.09.18.676967v2.full.pdf]
