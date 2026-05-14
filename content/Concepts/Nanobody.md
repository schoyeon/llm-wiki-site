---
aliases: [nanobody, nanobodies, VHH, single-domain antibody]
tags: [concept, antibody, protein]
sources: [The Virtual Lab_s41586-025-09442-9.pdf]
created: 2026-05-14
updated: 2026-05-14
---

# Nanobody

Single-domain antibody (VHH). 낙타과 동물의 heavy-chain-only antibody에서 유래한 ~15 kDa의 소형 항체 단편.

## Key Points

- 일반 항체 대비 크기가 작아 (~15 kDa vs ~150 kDa) 제조/엔지니어링이 용이
- ML 모델의 complexity도 낮출 수 있음 (자유도가 적음)
- 기존 nanobody를 mutation하여 새 variant에 대한 binding을 개선하는 전략이 de novo 설계보다 리스크가 낮음
- SARS-CoV-2 RBD에 결합하는 대표적 nanobody: Ty1, H11-D4, Nb21, VHH-72

## Virtual Lab에서의 활용

[[VirtualLab]]은 기존 Wuhan strain binder 4종을 input으로 받아, [[ESM]] + [[AlphaFoldMultimer]] + [[Rosetta]] pipeline으로 KP.3 variant binder를 설계함.

## Cross-References

- [[Swanson2025_VirtualLab|Virtual Lab 논문]]
- [[SARSCoV2]]
- [[VirtualLab]]

## Source Citations
- [The Virtual Lab_s41586-025-09442-9.pdf]
