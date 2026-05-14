---
aliases: [epitope prediction, B-cell epitope prediction, 에피토프 예측]
tags: [topic]
sources: []
created: 2026-05-14
updated: 2026-05-14
---

# Epitope Prediction

항원 표면에서 항체가 결합하는 영역(epitope)을 예측하는 분야. 항체 설계, 백신 개발에 핵심.

## 도구 비교

| 도구 | 방법 | 입력 | 특징 |
|-----|------|------|------|
| [[Hoie2024_DiscoTope3|DiscoTope-3.0]] | ESM-IF1 inverse folding | 구조 | AF2 predicted 구조에서도 작동 |
| [[Zeng2023_GraphBepi|GraphBepi]] | AF2 구조 + ESM-2 + EGNN | 구조+서열 | Graph-based |
| [[Tubiana2022_ScanNet|ScanNet]] | Geometric DL | 3D 좌표 | 해석 가능한 features |

## 관련 도구 (Binding Site / Hotspot)
- [[Krapp2023_PeSTo|PeSTo]] — parameter-free interface 예측
- [[Fang2023_DeepProSite|DeepProSite]] — 다중 결합 유형 지원
- [[Chen2024_PPIhotspot|PPI-hotspot]] — PPI hot spot 예측
- [[Zhao2026_Surf2Spot|Surf2Spot]] — nanobody design hotspot 예측

## Cross-References
- [[AntibodyDesign]]
- [[BindingSitePrediction]]
- [[Nanobody]]
