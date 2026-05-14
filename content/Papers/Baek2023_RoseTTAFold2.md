---
aliases: [RF2 paper, RoseTTAFold2 paper]
tags: [paper, structure-prediction]
sources: [rf2_2023.05.24.542179v1.full.pdf]
created: 2026-05-14
updated: 2026-05-14
---

# Efficient and accurate prediction of protein structure using RoseTTAFold2

**Authors:** Minkyung Baek, Ivan Anishchenko, Ian R. Humphreys, Qian Cong, David Baker, Frank DiMaio
**Source:** bioRxiv, 2023
**DOI:** 10.1101/2023.05.24.542179

## Summary

RoseTTAFold2 (RF2)는 RoseTTAFold와 AlphaFold2의 장점을 결합한 구조 예측 모델이다. 3-track 아키텍처(1D sequence, 2D pair, 3D structure)를 유지하면서 AF2의 recycling, FAPE loss, distillation을 도입했다. Monomer에서 AF2급 정확도를 달성하면서 complex 예측에서 더 나은 computational scaling을 보임. AF2의 핵심 기능(IPA, triangle attention) 없이도 높은 정확도 달성 가능함을 보여줌.

## Key Points

- **3-track architecture**: 1D (sequence/MSA) + 2D (pair) + 3D (structure) — 36 blocks 반복
- AF2의 Triangle attention 대신 SE3-equivariant transformer 사용
- Monomer: AF2와 동등, Complex: AF-Multimer보다 better scaling
- 코드와 모델 weights 공개 (오픈소스)
- [[Krishna2024_RoseTTAFoldAllAtom|RFAA]]의 기반 모델

## Cross-References

- [[Krishna2024_RoseTTAFoldAllAtom|RFAA 논문]]
- [[Jumper2021_AlphaFold2|AF2 논문]]
- [[StructurePrediction]]

## Source Citations
- [rf2_2023.05.24.542179v1.full.pdf]
