---
aliases: [LigandMPNN paper]
tags: [paper, protein-design, inverse-folding]
sources: [ligandmpnn_s41592-025-02626-1.pdf]
created: 2026-05-14
updated: 2026-05-14
---

# Atomic context-conditioned protein sequence design using LigandMPNN

**Authors:** Justas Dauparas, Gyu Rie Lee, Robert Pecoraro, Linna An, Ivan Anishchenko, Cameron Glasscock & David Baker
**Journal:** Nature Methods, Vol 22, 2025
**DOI:** 10.1038/s41592-025-02626-1

## Summary

LigandMPNN은 ProteinMPNN을 확장하여 소분자, 핵산, 금속 이온 등 비단백질 원자 컨텍스트를 모델링하는 서열 설계 도구이다. 3개의 그래프(protein backbone, atom-level, protein-ligand)를 사용. 소분자 상호작용 잔기 recovery 63.3% (vs ProteinMPNN 50.4%), 핵산 50.5% (vs 35.2%), 금속 77.5% (vs 36.0%). 100개 이상의 실험 검증된 소분자/DNA-binding 단백질 설계.

## Key Points

- **3-graph architecture**: protein backbone + atom-bond + protein-ligand
- Sidechain conformation도 출력 → binding interaction 평가 가능
- Rosetta 소분자 binder 재설계시 binding affinity 최대 100배 향상
- X-ray 결정 구조 4개로 높은 구조 정확도 확인
- ProteinMPNN 대비 비단백질 context에서 대폭 개선

## Cross-References

- [[Dauparas2022_ProteinMPNN|ProteinMPNN]] — 전신
- [[Watson2023_RFdiffusion|RFdiffusion]] — 파이프라인 연계
- [[Dreyer2023_AbMPNN|AbMPNN]]

## Source Citations
- [ligandmpnn_s41592-025-02626-1.pdf]
