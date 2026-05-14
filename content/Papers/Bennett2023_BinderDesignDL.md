---
aliases: [DL binder design paper]
tags: [paper, binder-design, deep-learning]
sources: [s41467-023-38328-5.pdf]
created: 2026-05-14
updated: 2026-05-14
---
# Improving de novo protein binder design with deep learning
**Authors:** Nathaniel R. Bennett, Brian Coventry, Inna Goreshnik, Buwei Huang, ..., David Baker
**Journal:** Nature Communications, 2023
**DOI:** 10.1038/s41467-023-38328-5
## Summary
AF2/RoseTTAFold를 활용하여 energy-based protein binder design의 성공률을 ~10배 향상시킨 연구. Designed sequence가 monomer structure를 채택하고 target에 결합할 확률을 AF2로 평가. ProteinMPNN이 Rosetta 대비 현저히 높은 computational efficiency.
## Key Points
- AF2/RF를 필터링에 활용 → design success rate ~10배 향상
- ProteinMPNN >> Rosetta for sequence design
- 13개 target에 대한 binder design 실험 검증
## Cross-References
- [[Cao2022_ProteinBinderDesign|Cao binder design]]
- [[Dauparas2022_ProteinMPNN|ProteinMPNN]]
- [[Watson2023_RFdiffusion|RFdiffusion]]
## Source Citations
- [s41467-023-38328-5.pdf]
