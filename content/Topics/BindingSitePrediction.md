---
aliases: [binding site prediction, pocket detection, 결합 사이트 예측]
tags: [topic]
sources: []
created: 2026-05-14
updated: 2026-05-14
---

# Binding Site & Pocket Prediction

단백질 표면에서 다른 분자(단백질, 리간드, 핵산 등)가 결합하는 영역을 예측하는 분야.

## 도구 분류

### Protein-Protein Interface 예측
| 도구 | 방법 | 특징 |
|-----|------|------|
| [[Krapp2023_PeSTo|PeSTo]] | Geometric transformer | Parameter-free, 다중 분자 유형 |
| [[Tubiana2022_ScanNet|ScanNet]] | Geometric DL | 해석 가능, antibody epitope 포함 |
| [[Fang2023_DeepProSite|DeepProSite]] | ESMFold + Graph Transformer | Unbound에서도 작동 |

### Hotspot 예측
| 도구 | 방법 | 특징 |
|-----|------|------|
| [[Chen2024_PPIhotspot|PPI-hotspot]] | FTMap + AF-M | Free structure만으로 예측 |
| [[Ngan2012_FTMAP|FTMAP]] | Fragment probe mapping | Physics-based, 웹 서버 |
| [[Zhao2026_Surf2Spot|Surf2Spot]] | Sequence+structure+surface | Nanobody design 연동 |

### Ligand Pocket Detection
| 도구 | 방법 | 특징 |
|-----|------|------|
| [[LeGuilloux2009_Fpocket|Fpocket]] | Voronoi + alpha spheres | 가장 널리 사용, 오픈소스 |
| [[Krivak2018_P2Rank|P2Rank]] | Random forest ML | Template-free, <1초 |
| [[Mareuil2025_InDeepNet|InDeepNet]] | DL + web platform | Ligandability 평가 포함 |

## Cross-References
- [[EpitopePrediction]]
- [[BinderDesign]]
- [[ProteinDesign]]
