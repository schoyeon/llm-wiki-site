---
aliases: [binder design, protein binder design, 바인더 설계]
tags: [topic]
sources: []
created: 2026-05-14
updated: 2026-05-14
---

# Protein Binder Design

Target 단백질에 결합하는 소형 단백질(miniprotein binder)을 de novo 설계하는 분야.

## 도구 비교

| 도구 | 방법 | Affinity | 특징 |
|-----|------|----------|------|
| [[Cao2022_ProteinBinderDesign|Cao 2022]] | RifGen/RifDock + Rosetta | pM-nM | Physics-based, <65aa |
| [[Bennett2023_BinderDesignDL|Bennett 2023]] | + AF2/RF 필터링 | nM | ~10x 성공률 향상 |
| [[Watson2023_RFdiffusion|RFdiffusion]] | Diffusion + hotspot | nM | Backbone 생성 혁신 |
| [[Pacesa2025_BindCraft|BindCraft]] | AF2 hallucination | pM-nM | End-to-end, 오픈소스 |
| [[Zambaldi2024_AlphaProteo|AlphaProteo]] | ML (DeepMind) | 80-960 pM | 최고 affinity |
| [[Sappington2024_BetaPairing|Beta-pairing]] | RFdiffusion + β-strand | 76 pM-nM | Polar surface 타겟 |
| [[VazquezTorres2024_PeptideBinders|Peptide binders]] | RFdiffusion + partial diffusion | pM | Helical peptide 타겟 |

## 면역 치료 응용
- [[Yang2025_ImmuneReceptorBinders|Immune receptor binders]] — TGFβRII, CTLA-4, PD-L1
- [[Balbi2026_Surfaceome|Surfaceome mapping]] — ~4,500 targetable sites on human surfaceome

## Hotspot 예측 (설계 전 단계)
- [[Zhao2026_Surf2Spot|Surf2Spot]] — binder design hotspot 예측, RFdiffusion/BindCraft 연동
- [[Chen2024_PPIhotspot|PPI-hotspot]] — free structure에서 hot spot 예측
- [[Ngan2012_FTMAP|FTMAP]] — fragment mapping으로 binding hot spot 탐지

## Cross-References
- [[ProteinDesign]]
- [[AntibodyDesign]]
- [[DiffusionModel]]
