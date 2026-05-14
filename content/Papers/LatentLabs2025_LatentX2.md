---
aliases: [Latent-X2 paper]
tags: [paper, antibody, protein-design, immunogenicity]
sources: [latent-x2_2512.20263v1.pdf]
created: 2026-05-14
updated: 2026-05-14
---

# Drug-like antibodies with low immunogenicity in human panels designed with Latent-X2

**Authors:** Latent Labs Team
**Source:** arXiv, 2025

## Summary

Latent-X2는 target structure + epitope specification으로부터 drug-like antibody를 zero-shot으로 설계하는 generative model이다. VHH, scFv, macrocyclic peptide 등 다양한 modality를 생성. AI 생성 항체 최초로 human donor panel에서 low immunogenicity를 확인. Picomolar~nanomolar binding affinity, 높은 developability (expression, stability, 낮은 polyreactivity).

## Key Points

- **Multi-modal**: VHH, scFv, macrocyclic peptide 모두 하나의 모델로 생성
- **최초 low immunogenicity 검증**: human donor panel에서 T-cell proliferation/cytokine assay
- All-atom model: target structure + epitope + optional framework 입력
- 4-24개 설계만으로 9/18 타겟 성공 (50% target-level success)
- K-Ras 대상 macrocyclic peptide — trillion-scale mRNA display와 경쟁 가능

## Cross-References

- [[Zambaldi2024_AlphaProteo|AlphaProteo]]
- [[Bennett2025_RFAntibody|RFAntibody]]
- [[MilleFragoso2025_Germinal|Germinal]]
- [[Nanobody]]

## Source Citations
- [latent-x2_2512.20263v1.pdf]
