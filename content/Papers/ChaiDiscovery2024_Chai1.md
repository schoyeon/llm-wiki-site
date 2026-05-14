---
aliases: [Chai-1 paper]
tags: [paper, structure-prediction]
sources: [chai-1_2024.10.10.615955v1.full.pdf]
created: 2026-05-14
updated: 2026-05-14
---

# Chai-1: Decoding the molecular interactions of life

**Authors:** Chai Discovery team
**Source:** bioRxiv, 2024
**DOI:** 10.1101/2024.10.10.615955

## Summary

Chai-1은 Chai Discovery에서 개발한 multi-modal foundation model로, 단백질-리간드, protein multimer 등 다양한 생체분자 구조 예측에서 SOTA를 달성. AF3와 유사한 diffusion 기반 아키텍처이지만, language model embedding, experimental constraint prompting (epitope mapping, cross-link mass spec 등) 기능을 추가. Single-sequence 모드에서 ESMFold를 능가하고 AF-M 2.3과 비슷한 성능.

## Key Points

- **AF3 스타일 아키텍처**: MSA module (4 blocks) → Pair-bias attention (48 blocks) → Diffusion (16 blocks)
- **Language model embedding**: 추가 input track으로 single-sequence 성능 향상
- **Constraint features**: pocket conditioning, epitope mapping, cross-link 등 실험 데이터 반영 가능
- **오픈소스**: weights + inference code 공개 (비상업적 용도)
- 상업적 사용: lab.chaidiscovery.com 웹 서버

## Cross-References

- [[Abramson2024_AlphaFold3|AF3 논문]] — 비교 대상
- [[StructurePrediction]]
- [[DiffusionModel]]
- [[ESM]]

## Source Citations
- [chai-1_2024.10.10.615955v1.full.pdf]
