---
aliases: [AF3 supplementary, AF3 methods]
tags: [paper, structure-prediction, deep-learning, supplementary]
sources: [af3sup_41586_2024_7487_MOESM1_ESM.pdf]
created: 2026-05-14
updated: 2026-05-14
---

# AlphaFold 3 — Supplementary Information

**Parent paper:** [[Abramson2024_AlphaFold3|AlphaFold 3 본문]]

## Contents Overview

이 supplementary는 AF3의 전체 아키텍처, 학습, inference를 pseudocode 수준으로 상세히 기술한 38페이지 문서.

### Data Pipeline (Section 2)
- Genetic search: Jackhmmer (UniProt), Nhmmer (RNA)
- MSA processing: paired + unpaired MSA
- Template search: hmmsearch against PDB
- Training data: Weighted PDB dataset + distillation datasets
- Tokenization: polymer는 residue 단위, ligand는 atom 단위
- Cropping: contiguous / spatial / spatial interface 3가지 전략

### Model Architecture (Section 3)
- **Input embedder**: single + pair representation 초기화
- **Relative position encoding**: chain 내/간 위치 인코딩
- **Sequence-local atom attention**: atom-level features 추출 (Algorithm 5-7)
- **MSA Module**: 4 blocks, pair-bias row-wise gated self-attention (Algorithm 8-10)
- **Triangle updates**: outgoing/incoming edges (Algorithm 12-13)
- **Triangle attention**: starting/ending node (Algorithm 14-15)
- **Pairformer stack**: 48 blocks (Algorithm 17)
- **Diffusion Module**: transformer-based U-Net, 원자 좌표 denoising (Algorithm 18-26)
  - DiffusionConditioning: Fourier embedding + AdaLN
  - DiffusionTransformer: AttentionPairBias + ConditionedTransitionBlock

### Confidence Heads (Section 4.3)
- **pLDDT**: per-atom predicted LDDT, 50 bins (Algorithm 31)
- **PAE**: predicted aligned error, 64 bins (0-32Å)
- **PDE**: predicted distance error
- **Experimentally resolved prediction**: per-atom 예측

### Training (Section 5)
- 3-stage training: initial → fine-tune 1 (crop 640) → fine-tune 2 (crop 768)
- Loss: smooth LDDT loss + diffusion loss + auxiliary losses
- Inference: 5 diffusion samples × multiple seeds → confidence ranking
- **Sample ranking**: 0.65 × ipTM + 0.1 × pTM + 0.25 × disorder (이전 AF-M과 다름)
- **Clash penalty**: 적용하여 최종 ranking

### Key Algorithms (31 pseudocode blocks)

| Algorithm | Name | 역할 |
|-----------|------|------|
| 1 | MainInferenceLoop | 전체 inference flow |
| 5-7 | AtomAttention Encoder/Decoder/Transformer | Atom-level feature 처리 |
| 8-10 | MSA Module | MSA row-wise attention |
| 12-15 | Triangle Multiplication/Attention | Pair representation update |
| 17 | PairformerStack | 핵심 48-block stack |
| 18-26 | Diffusion 관련 | 구조 생성 (noise → coordinates) |
| 27 | SmoothLDDTLoss | Training loss |
| 31 | ConfidenceHead | pLDDT, PAE, PDE 예측 |

## Cross-References

- [[Abramson2024_AlphaFold3|AF3 본문]]
- [[AlphaFold3]]
- [[DiffusionModel]]
- [[StructurePrediction]]

## Source Citations
- [af3sup_41586_2024_7487_MOESM1_ESM.pdf]
