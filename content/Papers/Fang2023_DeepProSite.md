---
aliases: [DeepProSite paper]
tags: [paper, binding-site-prediction]
sources: [deepProSite_btad718.pdf]
created: 2026-05-14
updated: 2026-05-14
---
# DeepProSite: structure-aware protein binding site prediction using ESMFold and pretrained language model
**Authors:** Yitian Fang, Yi Jiang, Leyi Wei, Qin Ma, Zhixiang Ren, Qianmu Yuan & Dong-Qing Wei
**Journal:** Bioinformatics, 2023
**DOI:** 10.1093/bioinformatics/btad718
## Summary
DeepProSite는 ESMFold 구조 + pretrained language model representation으로 protein binding site를 예측하는 도구. Graph Transformer로 binding site를 node classification. Protein-protein, protein-peptide, nucleic acid, ligand binding site 모두 예측 가능.
## Key Points
- ESMFold 구조 생성 → Graph Transformer로 binding site 예측
- Unbound structure에서도 높은 성능 유지
- 다중 결합 유형 지원 (protein, peptide, nucleic acid, ligand)
- 웹 서버: inner.wei-group.net/DeepProSite
## Cross-References
- [[Tubiana2022_ScanNet|ScanNet]]
- [[Krapp2023_PeSTo|PeSTo]]
## Source Citations
- [deepProSite_btad718.pdf]
