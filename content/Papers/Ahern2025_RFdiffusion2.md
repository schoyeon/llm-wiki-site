---
aliases: [RFdiffusion2 paper, RFD2]
tags: [paper, protein-design, enzyme-design, diffusion]
sources: [rfdiffusion2_s41592-025-02975-x.pdf]
created: 2026-05-14
updated: 2026-05-14
---

# Atom-level enzyme active site scaffolding using RFdiffusion2

**Authors:** Woody Ahern, Jason Yim, Doug Tischer, Saman Salike, ..., Rohith Krishna & David Baker
**Journal:** Nature Methods, 2025
**DOI:** 10.1038/s41592-025-02975-x

## Summary

RFdiffusion2는 원자 수준에서 효소 활성 부위를 직접 scaffold하는 diffusion 모델이다. 기존 RFdiffusion이 backbone 수준이었던 것과 달리, functional group의 기하학적 배치로부터 직접 효소를 설계한다. Residue order나 inverse rotamer 생성 없이 설계 가능. 다양한 벤치마크에서 41개 활성 부위 전부 scaffold 성공 (기존 방법: 16개).

## Key Points

- Backbone + side-chain atom 수준의 diffusion
- Functional group geometry → scaffold 직접 생성 (residue 순서 무관)
- 3가지 효소 촉매 메커니즘에 대해 활성 후보 설계 및 실험 검증
- 기존 motif scaffolding 대비 대폭 성능 향상 (41/41 vs 16/41)

## Cross-References

- [[Watson2023_RFdiffusion|RFdiffusion]] — 전신
- [[Butcher2025_RFdiffusion3|RFdiffusion3]] — 후속
- [[DiffusionModel]]

## Source Citations
- [rfdiffusion2_s41592-025-02975-x.pdf]
