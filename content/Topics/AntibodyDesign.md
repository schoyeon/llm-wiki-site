---
aliases: [antibody design, nanobody design, Ab design, 항체 설계]
tags: [topic]
sources: []
created: 2026-05-14
updated: 2026-05-14
---

# Antibody & Nanobody Design

항체/nanobody를 computational하게 de novo 설계하거나 기존 항체를 최적화하는 분야.

## 접근법 분류

| 접근법 | 도구 | 특징 |
|-------|------|------|
| De novo backbone+CDR | [[Bennett2025_RFAntibody|RFAntibody]] | RFdiffusion fine-tuned, epitope-targeted |
| Joint structure+sequence | [[MilleFragoso2025_Germinal|Germinal]] | AF-M + IgLM gradient 공동 최적화 |
| Inverse folding | [[Hoie2024_AntiFold|AntiFold]], [[Dreyer2023_AbMPNN|AbMPNN]] | 구조 → 서열 |
| Multi-modal generative | [[LatentLabs2025_LatentX2|Latent-X2]] | VHH/scFv/macrocycle, low immunogenicity |
| Mutation optimization | [[Swanson2025_VirtualLab|Virtual Lab]] | ESM + AF-M + Rosetta 파이프라인 |
| Agent-guided | [[Zhao2026_AgentNanobody|Agent nanobody]] | LLM agent 기반 워크플로우 |

## 핵심 이슈

- **CDR-H3**: 가장 가변적이고 중요한 루프 — 설계 난이도 높음
- **Epitope targeting**: 원하는 epitope에 정확히 결합하도록 설계
- **Developability**: binding뿐 아니라 expression, stability, immunogenicity 중요
- **Humanness**: 치료용 항체는 human germline 유사도 필요

## Docking & Benchmarking
- [[Hitawala2025_AF3AntibodyDocking|AF3 Ab docking benchmark]] — AF3의 항체 docking 성능
- [[Unsal2026_AntiConf|AntiConf]] — Ab-Ag complex confidence scoring

## 구조적 기초
- [[SelaCulang2013_AbAgRecognition|Ab-Ag recognition review]] — 항체-항원 인식 원리
- [[Herold2017_AbVariableDomains|Ab variable domains]] — VL/VH 조립과 기능

## Cross-References
- [[ProteinDesign]]
- [[BinderDesign]]
- [[Nanobody]]
- [[EpitopePrediction]]
