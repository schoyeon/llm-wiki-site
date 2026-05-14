---
aliases: [RFdiffusion paper]
tags: [paper, protein-design, diffusion]
sources: [rfdiffsuion_s41586-023-06415-8.pdf]
created: 2026-05-14
updated: 2026-05-14
---

# De novo design of protein structure and function with RFdiffusion

**Authors:** Joseph L. Watson, David Juergens, Nathaniel R. Bennett, Brian L. Trippe, ..., David Baker
**Journal:** Nature, Vol 620, 2023
**DOI:** 10.1038/s41586-023-06415-8

## Summary

RFdiffusion은 RoseTTAFold 구조 예측 네트워크를 fine-tuning하여 단백질 backbone을 de novo 생성하는 diffusion 모델이다. Unconditional/topology-constrained monomer design, binder design, symmetric oligomer design, enzyme active site scaffolding, motif scaffolding 등 광범위한 설계 과제를 해결. 수백 개의 설계 단백질을 실험적으로 검증하여 구조와 기능을 확인함.

## Key Points

- RoseTTAFold 구조 예측 네트워크를 denoising task로 fine-tuning
- **Backbone-level diffusion**: Cα 좌표 + orientation frames에 noise 추가/제거
- 설계 후 [[Dauparas2022_ProteinMPNN|ProteinMPNN]]으로 서열 설계 → AF2로 검증
- Binder design: hotspot residue conditioning으로 target에 결합하는 단백질 설계
- Symmetric design: cyclic, dihedral, tetrahedral 대칭 구조 생성
- 후속: [[Ahern2025_RFdiffusion2|RFdiffusion2]], [[Butcher2025_RFdiffusion3|RFdiffusion3]]

## Cross-References

- [[Dauparas2022_ProteinMPNN|ProteinMPNN]] — 서열 설계
- [[Ahern2025_RFdiffusion2|RFdiffusion2]]
- [[Butcher2025_RFdiffusion3|RFdiffusion3]]
- [[DiffusionModel]]
- [[StructurePrediction]]

## Source Citations
- [rfdiffsuion_s41586-023-06415-8.pdf]
