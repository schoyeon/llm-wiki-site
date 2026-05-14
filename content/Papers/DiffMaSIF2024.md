---
aliases: [DiffMaSIF paper]
tags: [paper, protein-docking, diffusion, surface]
sources: [7368_DiffMaSIF_Score_Based_Dif.pdf]
created: 2026-05-14
updated: 2026-05-14
---
# DiffMaSIF: Score-Based Diffusion Models for Protein Surfaces
**Authors:** Anonymous (ICLR 2024 submission)
**Source:** ICLR 2024
## Summary
DiffMaSIF는 protein surface의 geometric/chemical features를 활용한 score-based diffusion 모델로, rigid-body protein-protein docking을 수행. Co-evolution 정보 없이도 structurally novel interface와 low sequence conservation 케이스에서 SOTA 달성.
## Key Points
- Surface point cloud + geometrically pre-trained residue embeddings
- Contact site prediction을 pretraining + auxiliary loss로 학습
- SO(3) diffusion으로 rigid-body docking (rotation + translation 예측)
- Low co-evolution interface에서 특히 강점
## Cross-References
- [[DiffusionModel]]
- [[StructurePrediction]]
## Source Citations
- [7368_DiffMaSIF_Score_Based_Dif.pdf]
