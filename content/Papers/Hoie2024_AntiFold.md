---
aliases: [AntiFold paper]
tags: [paper, antibody, inverse-folding]
sources: [antifold_vbae202.pdf]
created: 2026-05-14
updated: 2026-05-14
---

# AntiFold: improved structure-based antibody design using inverse folding

**Authors:** Magnus Haraldson Høie, Alissa M. Hummer, Tobias H. Olsen, Broncio Aguilar-Sanjuan, Morten Nielsen & Charlotte M. Deane
**Journal:** Bioinformatics Advances, 2025
**DOI:** 10.1093/bioadv/vbae202

## Summary

AntiFold는 ESM-IF1을 항체 구조에 fine-tuning한 antibody-specific inverse folding 모델이다. SAbDab + OAS 데이터로 학습하여 CDR 영역, 특히 CDR-H3에서 기존 도구(ProteinMPNN, AbMPNN) 대비 향상된 sequence recovery를 달성. Binding affinity 예측과 structural tolerance 평가 기능도 제공.

## Key Points

- ESM-IF1 기반 → antibody 데이터로 fine-tuning
- CDR-H3 AAR (Amino Acid Recovery) 31.5% (validation set)
- Zero-shot binding affinity prediction 가능
- Residue probability + structural tolerance + inverse folding 4가지 output
- 오픈소스: GitHub (oxpig/AntiFold)

## Cross-References

- [[Dreyer2023_AbMPNN|AbMPNN]]
- [[Dauparas2022_ProteinMPNN|ProteinMPNN]]
- [[Nanobody]]

## Source Citations
- [antifold_vbae202.pdf]
