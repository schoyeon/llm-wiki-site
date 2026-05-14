---
aliases: [AntiConf paper]
tags: [paper, antibody, confidence-scoring, benchmark]
sources: [bbag137.pdf]
created: 2026-05-14
updated: 2026-05-14
---
# Confidence scoring for deep learning-predicted antibody-antigen complexes: AntiConf as a precision-driven metric
**Authors:** Serbülent Ünsal, Benjamin Holland, Inci Sardag & Emel Timucin
**Journal:** Briefings in Bioinformatics, 2026
**DOI:** 10.1093/bib/bbag137
## Summary
Ab-Ag complex prediction 도구들 (AF2, Boltz-1x, Chai-1, Protenix 등)의 confidence score를 체계적으로 벤치마크. pDockQ2와 pTM score를 통합한 AntiConf metric을 개발하여, precision/recall에서 기존 개별 metric 대비 우수한 성능. Protenix-1이 전반적으로 가장 좋은 성능.
## Key Points
- 200개 Ab-Ag complex benchmark (SAbDab 기반)
- 9개 method 비교: AF2, Boltz-1x, Chai-1, Protenix-1, OpenFold3, ESMFold
- **AntiConf** = pDockQ2 + pTM 통합 metric
- Protenix-1이 overall top performer, Chai-1이 2위
## Cross-References
- [[AlphaFold3]]
- [[Hitawala2025_AF3AntibodyDocking|AF3 Ab docking benchmark]]
- [[ChaiDiscovery2024_Chai1|Chai-1]]
## Source Citations
- [bbag137.pdf]
