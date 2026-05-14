---
aliases: [Agent-guided nanobody paper]
tags: [paper, nanobody, agent, cancer]
sources: [2026.04.13.717816v1.full.pdf]
created: 2026-05-14
updated: 2026-05-14
---
# Agent-Guided De Novo Design of Nanobody Binders Against a Novel Cancer Target
**Authors:** Yue Zhao, Melih Yilmaz, Edward Lee, Chuanyui Teh, ..., Nai-Kong V Cheung, Jiwon Kim & Xinyun (Nina) Cheng
**Source:** bioRxiv, 2026 (Amazon Web Services + Memorial Sloan Kettering)
**DOI:** 10.64898/2026.04.13.717816
## Summary
Novel cancer target (Desmoplastic Small Round Cell Tumor)에 대한 agent-guided nanobody 설계 워크플로우. (1) Hotspot recommendation agent (IEDB, PFAM) → (2) RFAntibody/IgGM/mBER로 de novo nanobody 생성 → (3) Multi-metric scoring → (4) YSD screening + SPR. 288,000 nanobody 설계, 100,000 YSD 스크리닝 → 46/116 (39.7%) reliable binder, Kd 0.66-305 nM.
## Key Points
- **Agent-guided**: LLM agent가 hotspot 추천, epitope 선택 자동화
- 3개 VHH framework × 8 epitope × 3 generation methods
- Multi-objective Pareto filtering → YSD + FACS → SPR
- 39.7% hit rate, median Kd 31.7 nM
- Novel target (DSRCT) — 구조 정보/기존 항체 없음
## Cross-References
- [[Bennett2025_RFAntibody|RFAntibody]]
- [[Swanson2025_VirtualLab|Virtual Lab]] — 유사한 agent-guided 접근
- [[Nanobody]]
- [[MultiAgentLLM]]
## Source Citations
- [2026.04.13.717816v1.full.pdf]
