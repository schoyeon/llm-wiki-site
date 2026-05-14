---
aliases: [BindCraft paper]
tags: [paper, protein-design, binder-design]
sources: [One-shot_design_of_functional_protein_binders_with_BindCraft.pdf]
created: 2026-05-14
updated: 2026-05-14
---

# One-shot design of functional protein binders with BindCraft

**Authors:** Martin Pacesa, Lennart Nickel, Christian Schellhass, ..., Sergey Ovchinnikov & Bruno E. Correia
**Journal:** Nature, Vol 646, 2025
**DOI:** 10.1038/s41586-025-09429-6

## Summary

BindCraft는 AF2 weights를 활용한 오픈소스 de novo protein binder 설계 파이프라인이다. AF2를 backpropagation하여 binder backbone+sequence를 동시 생성하고, MPNN으로 최적화 후 AF2 monomer로 필터링. 12개 diverse target에 대해 10-100% 실험 성공률, nanomolar~picomolar affinity 달성. RFdiffusion과 달리 high-throughput screening 없이도 동작.

## Key Points

- AF2 hallucination을 활용: error gradient로 binder structure+sequence 동시 생성
- 12개 타겟: cell-surface receptors, allergens, de novo proteins, multi-domain nucleases
- 실험 성공률 10-100%, Kd: <1 nM ~ 120 nM
- RFdiffusion 대비: backbone을 고정하지 않고 매 iteration마다 flexible하게 재생성
- 오픈소스, minimal user intervention

## Cross-References

- [[Zambaldi2024_AlphaProteo|AlphaProteo]]
- [[Cao2022_ProteinBinderDesign|Cao et al. binder design]]
- [[Watson2023_RFdiffusion|RFdiffusion]]
- [[Dauparas2022_ProteinMPNN|ProteinMPNN]]

## Source Citations
- [One-shot_design_of_functional_protein_binders_with_BindCraft.pdf]
