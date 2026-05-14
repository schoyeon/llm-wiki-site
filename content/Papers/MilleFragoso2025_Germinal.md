---
aliases: [Germinal paper]
tags: [paper, antibody, protein-design, epitope]
sources: [germinal_2025.09.19.677421v1.full.pdf]
created: 2026-05-14
updated: 2026-05-14
---

# Efficient generation of epitope-targeted de novo antibodies with Germinal

**Authors:** Luis S. Mille-Fragoso, John N. Wang, Claudia L. Driscoll, Haoyu Dai, Talal Widatalla, Xiaowei Zhang, Brian L. Hie & Xiaojing J. Gao
**Source:** bioRxiv, 2025
**DOI:** 10.1101/2025.09.19.677421

## Summary

Germinal은 사용자가 지정한 epitope에 결합하는 항체/nanobody를 de novo 설계하는 generative framework이다. AlphaFold-Multimer (structure) + IgLM (antibody sequence prior)의 gradient를 공동 최적화하여 CDR 서열을 설계. 4개 타겟(PD-L1, IL3, IL20, BHRF1)에 대해 43-101개 설계 중 4-22% 실험 성공률 달성, nanomolar binding affinity 확인.

## Key Points

- **Joint optimization**: AF-M confidence + IgLM likelihood → CDR sequence 최적화
- 3-phase: Logits → Softmax (temperature annealing) → Semi-greedy
- Single-domain antibody (VHH) + nanobody 설계 가능
- BLI 검증: best Kd 140-560 nM
- 오픈소스 코드 + 실험 프로토콜 공개

## Cross-References

- [[AlphaFoldMultimer]]
- [[Bennett2025_RFAntibody|RFAntibody]]
- [[Nanobody]]

## Source Citations
- [germinal_2025.09.19.677421v1.full.pdf]
