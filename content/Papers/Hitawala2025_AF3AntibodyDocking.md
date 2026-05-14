---
aliases: [AF3 antibody docking benchmark]
tags: [paper, antibody, structure-prediction, benchmark]
sources: [KMAB_17_2545601.pdf]
created: 2026-05-14
updated: 2026-05-14
---

# What does AlphaFold3 learn about antibody and nanobody docking, and what remains unsolved?

**Authors:** Fatima N. Hitawala & Jeffrey J. Gray
**Journal:** mAbs, Vol 17, 2025
**DOI:** 10.1080/19420862.2025.2545601

## Summary

AF3의 항체/nanobody docking 성능을 체계적으로 벤치마킹한 논문. SAbDab에서 curated benchmark를 구성하여 AF3, AF2.3-M, Boltz-1, Chai-1을 비교. AF3가 1 seed에서 10.2% (antibody) / 13.3% (nanobody) high-accuracy success rate 달성. 20 seed에서 향상되지만, CDR-H3 모델링이 여전히 주요 한계. ipTM·HA + ΔGb 조합이 최적 ranking protocol.

## Key Points

- AF3: DockQ > 0.23 success rate 34.7% (antibody), AF-M 2.3 대비 개선
- CDR-H3 accuracy: 2.08-2.71 Å (antibodies), 3.78-3.63 Å (nanobodies)
- **Nanobody docking이 antibody보다 어려움** (CDR-H3 비중 높음)
- Antigen context (bound vs unbound) 제공 시 CDR-H3 accuracy 향상
- Boltz-1, Chai-1: 전반적으로 AF3보다 낮은 성능

## Cross-References

- [[AlphaFold3]]
- [[Abramson2024_AlphaFold3|AF3 논문]]
- [[Nanobody]]
- [[ChaiDiscovery2024_Chai1|Chai-1]]

## Source Citations
- [KMAB_17_2545601.pdf]
