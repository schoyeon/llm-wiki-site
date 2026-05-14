---
aliases: [ProteinMPNN, MPNN]
tags: [entity, tool, protein-design, inverse-folding]
sources: []
created: 2026-05-14
updated: 2026-05-14
---
# ProteinMPNN
단백질 backbone 구조 → 아미노산 서열을 설계하는 inverse folding 모델. David Baker 그룹 (UW).
## Key Points
- Message-passing neural network 기반
- Backbone N/Cα/C/O 좌표 입력 → 서열 출력 (autoregressive)
- RFdiffusion 파이프라인의 핵심 서열 설계 단계
- 후속 확장: [[Dauparas2025_LigandMPNN|LigandMPNN]], [[Dreyer2023_AbMPNN|AbMPNN]]
## Cross-References
- [[Dauparas2022_ProteinMPNN|논문]]
- [[RFdiffusion]] — backbone 생성
- [[ProteinDesign]]
