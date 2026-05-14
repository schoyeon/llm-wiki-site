---
aliases: [Cao binder design paper]
tags: [paper, protein-design, binder-design]
sources: [Design_of_protein-binding_proteins_from_the_target_structure_alone.pdf]
created: 2026-05-14
updated: 2026-05-14
---

# Design of protein-binding proteins from the target structure alone

**Authors:** Longxing Cao, Brian Coventry, Inna Goreshnik, ..., David Baker
**Journal:** Nature, Vol 605, 2022
**DOI:** 10.1038/s41586-022-04654-9

## Summary

Target 단백질의 3D 구조만으로 de novo protein binder를 설계하는 general approach. RifGen/RifDock로 hotspot side-chain 배치 → Rosetta로 scaffold 도킹 → ProteinMPNN 서열 설계. 12개 diverse target에 대해 <65 aa 크기의 binder 설계, nanomolar~picomolar affinity 달성. 5개의 crystal structure로 computational model과의 일치 확인.

## Key Points

- **2-stage**: (1) RifGen/RifDock으로 target surface에 hotspot side-chain 배치, (2) scaffold 도킹
- Nearly 1M computational designs → hundreds of thousands의 point mutant 실험 데이터
- 12개 타겟에 대해 binder 설계 성공
- 65 aa 미만, hyperstable, nanomolar-picomolar affinity
- RFdiffusion 이전의 physics-based binder design 대표작

## Cross-References

- [[Pacesa2025_BindCraft|BindCraft]] — 후속 AF2 기반 방법
- [[Zambaldi2024_AlphaProteo|AlphaProteo]]
- [[Watson2023_RFdiffusion|RFdiffusion]]
- [[Rosetta]]

## Source Citations
- [Design_of_protein-binding_proteins_from_the_target_structure_alone.pdf]
