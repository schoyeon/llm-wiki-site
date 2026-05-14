---
aliases: [Virtual Lab, Virtual Lab paper]
tags: [paper, nanobody, multi-agent, LLM]
sources: [The Virtual Lab_s41586-025-09442-9.pdf]
created: 2026-05-14
updated: 2026-05-14
---

# The Virtual Lab of AI agents designs new SARS-CoV-2 nanobodies

**Authors:** Kyle Swanson, Wesley Wu, Nash L. Bulaong, John E. Pak, James Zou
**Journal:** Nature, Vol 646, 16 October 2025
**DOI:** 10.1038/s41586-025-09442-9

## Summary

Virtual Lab은 LLM 기반 multi-agent 시스템으로, AI-human 협업을 통해 학제간 연구를 수행한다. Human researcher가 LLM Principal Investigator(PI)와 여러 specialist agent들을 이끌며, 연구 회의(team meeting + individual meeting)를 통해 연구를 진행한다. SARS-CoV-2 KP.3 variant에 결합하는 nanobody 92개를 설계했으며, 실험 검증에서 90% 이상이 발현되고 가용성을 보였다. JN.1/KP.3 spike RBD에 대한 결합 프로파일을 가진 2개의 후보가 확인되었다.

## Key Points

- **Architecture**: Human researcher → PI agent → Scientific Critic + specialist agents (Immunologist, ML Specialist, Computational Biologist)
- **Two meeting types**: Team meeting (broad discussion, N rounds) + Individual meeting (specific task, critique loop)
- **Parallel meetings**: 동일 agenda를 다른 temperature로 5회 병렬 실행 → merge하여 robustness 확보
- **Nanobody pipeline**: [[ESM]] LLR로 mutation 제안 → [[AlphaFoldMultimer]] ipLDDT로 구조 평가 → [[Rosetta]] dG로 binding energy 계산
- **Weighted Score**: WS = 0.2 × ESM LLR^WT + 0.5 × AF ipLDDT - 0.3 × RS dG
- **4 rounds of optimization**: 각 round에서 top 5 선택 → 다음 round input으로 사용
- **Input nanobodies**: Ty1, H11-D4, Nb21, VHH-72 (기존 Wuhan strain binder)
- **결과**: 92개 mutant 중 90%+ 발현, 2개(JN.1/KP.3 binding 확인)가 유망 후보
- **코드**: `virtual-lab` Python package (GitHub: zou-group/virtual-lab)

## Computational Pipeline Details

| Step | Tool | Metric | 역할 |
|------|------|--------|-----|
| Mutation 제안 | [[ESM]] | LLR (Log-Likelihood Ratio) | Sequence fitness 평가 |
| 구조 예측 | [[AlphaFoldMultimer]] | ipLDDT (interface pLDDT) | 결합 interface 품질 |
| Binding energy | [[Rosetta]] | RS dG (separated dG) | 열역학적 결합 안정성 |

### Scoring Formula
```
WS = 0.2 × (ESM LLR) + 0.5 × (AF ipLDDT) − 0.3 × (RS dG)
```
- ESM LLR^WT: mutant vs wildtype 비교 ratio
- 4 rounds × 5 inputs = 총 92 nanobodies (23 per input × 4 inputs)

## Experimental Validation

| Nanobody | ESM LLR^WT | AF ipLDDT | RS dG | WS^WT |
|----------|-----------|-----------|-------|-------|
| Ty1 (WT) | 0.00 | 71.83 | -41.51 | 48.36 |
| Ty1 V32F-G59D-N54S-F32S | 3.51 | 86.06 | -28.69 | 52.34 |
| H11-D4 (WT) | 0.00 | 68.18 | -38.93 | 45.77 |
| H11-D4 A14P-Y88V-K74T-R27L | 10.67 | 84.02 | -35.04 | 54.66 |
| Nb21 (WT) | 0.00 | 72.11 | -43.32 | 49.05 |
| Nb21 I77V-L59E-Q87A-R37Q | 7.47 | 80.41 | -51.56 | 57.17 |
| VHH-72 (WT) | 0.00 | 66.46 | -20.90 | 39.50 |
| VHH-72 R27Y-E31D-F37V-D89E | 8.82 | 69.51 | -53.76 | 52.65 |

- 96개 nanobody 발현 테스트: 90%+ soluble expression
- ELISA binding: H11-D4 variants, Nb21 variants가 Wuhan RBD에 strong binding
- **2개 후보 (JN.1, KP.3 binding)**: cross-variant reactivity 확인

## Cross-References

- [[VirtualLab]] — 시스템 아키텍처 상세
- [[ESM]] — protein language model
- [[AlphaFoldMultimer]] — 구조 예측
- [[Rosetta]] — energy 계산
- [[Nanobody]] — nanobody 개념
- [[SARSCoV2]] — target virus
- [[JamesZou]] — corresponding author
- [[MultiAgentLLM]] — multi-agent 패턴

## Source Citations
- [The Virtual Lab_s41586-025-09442-9.pdf] — full paper
