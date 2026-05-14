---
aliases: [ProteinMPNN paper]
tags: [paper, protein-design, inverse-folding]
sources: [proteinmpnn_science.add2187.pdf]
created: 2026-05-14
updated: 2026-05-14
---

# Robust deep learning-based protein sequence design using ProteinMPNN

**Authors:** J. Dauparas, I. Anishchenko, N. Bennett, H. Baek, ..., D. Baker
**Journal:** Science, Vol 378, 2022
**DOI:** 10.1126/science.add2187

## Summary

ProteinMPNN은 단백질 backbone 구조로부터 아미노산 서열을 설계하는 inverse folding 모델이다. Message-passing neural network (MPNN)으로 backbone의 N, Cα, C, O 좌표와 Cβ 거리를 인코딩하고, autoregressive decoder로 서열을 생성. Rosetta 대비 현저히 높은 sequence recovery와 실험 성공률을 달성. Monomer 52%, heteromer 51% median sequence recovery.

## Key Points

- **Backbone Encoder**: 3-layer MPNN, N/Cα/C/O 좌표 + Cβ 거리 → node/edge features
- **Sequence Decoder**: autoregressive, random decoding order 지원
- Tied positions: symmetric design, multistate design 가능
- Backbone noise (σ=0.02Å) 추가시 AF2 predicted structure에서 더 나은 성능
- [[Watson2023_RFdiffusion|RFdiffusion]] 파이프라인의 핵심 서열 설계 단계

## Cross-References

- [[Watson2023_RFdiffusion|RFdiffusion]] — backbone → ProteinMPNN → AF2 검증
- [[Dauparas2025_LigandMPNN|LigandMPNN]] — 후속 확장 모델
- [[Dreyer2023_AbMPNN|AbMPNN]] — 항체 특화 버전
- [[Goverde2024_SolubleMPNN|SolubleMPNN]]

## Source Citations
- [proteinmpnn_science.add2187.pdf]
