---
aliases: [Index, MOC]
tags: [index]
created: 2026-05-14
updated: 2026-05-14
---

# Master Index

## Topics
- [[ProteinDesign]] — 단백질 설계 (RFdiffusion, ProteinMPNN 파이프라인)
- [[AntibodyDesign]] — 항체/nanobody 설계 (RFAntibody, Germinal, Latent-X2)
- [[BinderDesign]] — protein binder 설계 (BindCraft, AlphaProteo)
- [[EpitopePrediction]] — B-cell epitope 예측 (DiscoTope, GraphBepi)
- [[BindingSitePrediction]] — 결합 사이트/pocket 예측 (PeSTo, Fpocket, P2Rank)
- [[SARSCoV2]] — SARS-CoV-2 / COVID-19

## Entities — Tools
- [[RFdiffusion]] — diffusion 기반 단백질 backbone 생성
- [[ProteinMPNN]] — inverse folding 서열 설계
- [[BindCraft]] — AF2 기반 end-to-end binder 설계
- [[AlphaProteo]] — DeepMind binder 설계
- [[AlphaFold3]] — 범용 생체분자 구조 예측
- [[AlphaFoldMultimer]] — protein complex 구조 예측
- [[ESM]] — protein language model (Meta AI)
- [[Rosetta]] — 단백질 에너지 계산
- [[VirtualLab]] — AI-human 협업 multi-agent 프레임워크

## Entities — People
- [[DavidBaker]] — UW IPD, 2024 노벨 화학상
- [[DemisHassabis]] — DeepMind CEO, 2024 노벨 화학상
- [[JohnJumper]] — AlphaFold lead, 2024 노벨 화학상
- [[JamesZou]] — Stanford CS, Virtual Lab

## Concepts
- [[Nanobody]] — single-domain antibody (VHH)
- [[MultiAgentLLM]] — multi-agent LLM 시스템
- [[DiffusionModel]] — 생성 모델 (AF3, RFdiffusion 핵심)
- [[StructurePrediction]] — 구조 예측 개념 및 도구 계보

## Papers (48)

### Structure Prediction
- [[Jumper2021_AlphaFold2|AlphaFold 2]] · [[Abramson2024_AlphaFold3|AlphaFold 3]] · [[Abramson2024_AlphaFold3_Supplement|AF3 Supplement]]
- [[Baek2023_RoseTTAFold2|RoseTTAFold2]] · [[Krishna2024_RoseTTAFoldAllAtom|RFAA]] · [[ChaiDiscovery2024_Chai1|Chai-1]] · [[Kim2025_ColabFold|ColabFold]]

### Protein Design & Inverse Folding
- [[Watson2023_RFdiffusion|RFdiffusion]] · [[Ahern2025_RFdiffusion2|RFdiffusion2]] · [[Butcher2025_RFdiffusion3|RFdiffusion3]]
- [[Dauparas2022_ProteinMPNN|ProteinMPNN]] · [[Dauparas2025_LigandMPNN|LigandMPNN]] · [[Goverde2024_SolubleMPNN|SolubleMPNN]] · [[Dreyer2023_AbMPNN|AbMPNN]]

### Antibody & Nanobody Design
- [[Bennett2025_RFAntibody|RFAntibody]] · [[Bennett2025_RFAntibody_Supplement|RFAntibody Supplement]]
- [[Hoie2024_AntiFold|AntiFold]] · [[MilleFragoso2025_Germinal|Germinal]] · [[LatentLabs2025_LatentX2|Latent-X2]]
- [[Hitawala2025_AF3AntibodyDocking|AF3 Ab Docking]] · [[Unsal2026_AntiConf|AntiConf]]
- [[Swanson2025_VirtualLab|Virtual Lab]] · [[Zhao2026_AgentNanobody|Agent Nanobody]]
- [[Xu2025_VHH_LGR5|VHH LGR5]]

### Binder Design
- [[Cao2022_ProteinBinderDesign|Cao 2022]] · [[Bennett2023_BinderDesignDL|Bennett 2023 DL]] · [[Pacesa2025_BindCraft|BindCraft]] · [[Zambaldi2024_AlphaProteo|AlphaProteo]]
- [[Sappington2024_BetaPairing|Beta-pairing]] · [[VazquezTorres2024_PeptideBinders|Peptide binders]] · [[Yang2025_ImmuneReceptorBinders|Immune receptors]]
- [[Balbi2026_Surfaceome|Surfaceome]]

### Epitope & Binding Site Prediction
- [[Hoie2024_DiscoTope3|DiscoTope-3.0]] · [[Zeng2023_GraphBepi|GraphBepi]] · [[Tubiana2022_ScanNet|ScanNet]]
- [[Krapp2023_PeSTo|PeSTo]] · [[Fang2023_DeepProSite|DeepProSite]] · [[Mareuil2025_InDeepNet|InDeepNet]]
- [[Chen2024_PPIhotspot|PPI-hotspot]] · [[Ngan2012_FTMAP|FTMAP]] · [[Zhao2026_Surf2Spot|Surf2Spot]]
- [[LeGuilloux2009_Fpocket|Fpocket]] · [[Krivak2018_P2Rank|P2Rank]]

### Other
- [[DiffMaSIF2024|DiffMaSIF]] · [[Yang2026_StructuralOntogeny|Structural Ontogeny]]
- [[Garcia2026_ZeroShotDesignSuccess|Zero-shot Design Success]] · [[SelaCulang2013_AbAgRecognition|Ab-Ag Recognition]] · [[Herold2017_AbVariableDomains|Ab Variable Domains]]
