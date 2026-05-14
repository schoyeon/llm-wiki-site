---
aliases: [protein design, de novo protein design, 단백질 설계]
tags: [topic]
sources: []
created: 2026-05-14
updated: 2026-05-14
---

# Protein Design

구조와 기능을 갖춘 단백질을 computational하게 설계하는 분야. Backbone 생성 → 서열 설계 → 구조 검증의 3단계 파이프라인이 표준.

## 표준 파이프라인

```
Backbone 생성 (RFdiffusion) → 서열 설계 (ProteinMPNN) → 구조 검증 (AF2/RF2)
```

## 핵심 도구 계보

| 세대 | Backbone 생성 | 서열 설계 | 검증 |
|------|-------------|--------|------|
| 전통 | Rosetta (physics) | Rosetta | X-ray |
| 1세대 DL | [[Watson2023_RFdiffusion|RFdiffusion]] | [[Dauparas2022_ProteinMPNN|ProteinMPNN]] | [[Jumper2021_AlphaFold2|AF2]] |
| 2세대 DL | [[Ahern2025_RFdiffusion2|RFdiffusion2]] | [[Dauparas2025_LigandMPNN|LigandMPNN]] | [[AlphaFold3|AF3]] |
| 3세대 DL | [[Butcher2025_RFdiffusion3|RFdiffusion3]] | — | — |
| End-to-end | [[Pacesa2025_BindCraft|BindCraft]], [[Zambaldi2024_AlphaProteo|AlphaProteo]] | (통합) | (통합) |

## 관련 논문

### Backbone 생성
- [[Watson2023_RFdiffusion|RFdiffusion]] — diffusion 기반 backbone 생성의 시작
- [[Ahern2025_RFdiffusion2|RFdiffusion2]] — atom-level enzyme active site scaffolding
- [[Butcher2025_RFdiffusion3|RFdiffusion3]] — all-atom biomolecular design

### 서열 설계 (Inverse Folding)
- [[Dauparas2022_ProteinMPNN|ProteinMPNN]] — backbone → sequence
- [[Dauparas2025_LigandMPNN|LigandMPNN]] — 비단백질 context 포함
- [[Goverde2024_SolubleMPNN|SolubleMPNN]] — membrane protein analogues

### 설계 성공률 평가
- [[Garcia2026_ZeroShotDesignSuccess|Garcia 2026]] — AF2/ESMFold/ProteinMPNN으로 설계 성공 예측
- [[Goverde2024_SolubleMPNN|SolubleMPNN]] — 새로운 fold의 soluble 단백질 설계

## Cross-References
- [[BinderDesign]]
- [[AntibodyDesign]]
- [[DiffusionModel]]
- [[StructurePrediction]]
