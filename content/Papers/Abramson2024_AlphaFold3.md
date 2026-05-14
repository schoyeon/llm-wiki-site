---
aliases: [AF3 paper, AlphaFold 3 paper]
tags: [paper, structure-prediction, deep-learning]
sources: [alphafold3_s41586-024-07487-w.pdf]
created: 2026-05-14
updated: 2026-05-14
---

# Accurate structure prediction of biomolecular interactions with AlphaFold 3

**Authors:** Josh Abramson, Jonas Adler, Jack Dunger, Richard Evans, Tim Green, Alexander Pritzel, Olaf Ronneberger, Lindsay Willmore, ..., Demis Hassabis & John M. Jumper
**Journal:** Nature, Vol 630, 13 June 2024
**DOI:** 10.1038/s41586-024-07487-w

## Summary

AlphaFold 3 (AF3)는 단백질뿐 아니라 핵산, 소분자(리간드), 이온, 변형 잔기를 포함한 거의 모든 생체분자 복합체의 3D 구조를 예측하는 통합 딥러닝 모델이다. AF2의 Evoformer를 간소화한 Pairformer와, structure module을 대체하는 diffusion module이 핵심 아키텍처 변화다. PDB의 거의 모든 분자 유형에서 SOTA를 달성했으며, 특히 protein-ligand, protein-nucleic acid, antibody-antigen 예측에서 큰 개선을 보였다.

## Key Points

- **AF2 대비 핵심 변화**: Structure module → Diffusion module (노이즈 제거 방식으로 원자 좌표 직접 예측)
- **Pairformer**: Evoformer에서 MSA processing을 최소화하고, pair representation 중심으로 단순화 (48 blocks)
- **입력**: 단백질, DNA, RNA, 리간드, 이온, 공유 변형(인산화 등) 모두 가능
- **Confidence metrics**: pLDDT (per-residue), pTM, ipTM, PAE (Predicted Aligned Error)
- **DockQ > 0.23** = correct prediction, **DockQ > 0.8** = very high accuracy
- Antibody-antigen 예측: AF-M 2.3 대비 **대폭 개선**, seed 수 증가시 품질 향상 지속
- **AlphaFold Server**: alphafoldserver.com에서 무료 사용 가능

## Architecture

```
Inputs (sequences, ligands, ions)
    ↓
Template module (2 blocks)
    ↓
MSA module (4 blocks) — 대폭 축소
    ↓
Pairformer (48 blocks) — AF3의 핵심
    ↓
Diffusion module (원자 좌표 직접 예측)
    ↓
Confidence module (pLDDT, pTM, PAE)
```

### Diffusion Module
- 노이즈가 추가된 원자 좌표에서 시작 → 반복적으로 denoising하여 최종 구조 예측
- Rotational frames이나 equivariant processing 불필요
- Training: 스테레오케미컬 violation penalties로 화학적 타당성 강제
- Inference: 여러 seed로 multiple samples 생성 → confidence로 ranking

## Performance Benchmarks

| Category | Metric | AF3 | AF-M 2.3 | 비교 |
|----------|--------|-----|----------|-----|
| Protein-protein | DockQ | SOTA | baseline | AF3 > AF-M 2.3 |
| Protein-ligand | % RMSD < 2Å | 76.1% | — | >> Vina, DiffDock 등 |
| Protein-DNA | LDDT | ~80 | ~73 | 큰 개선 |
| Protein-RNA | LDDT | ~70 | ~64 | 큰 개선 |
| Antibody-antigen | DockQ | 대폭 향상 | baseline | seed 증가시 지속 개선 |
| Covalent modifications | 인산화 등 | 지원 | 미지원 | 새 기능 |

### Confidence Metrics 상세

| Metric | 정의 | 용도 |
|--------|-----|------|
| **pLDDT** | per-residue Local Distance Difference Test | 잔기별 구조 신뢰도 |
| **pTM** | predicted Template Modeling score | 전체 구조 품질 |
| **ipTM** | interface pTM (chain pair) | 두 chain 간 결합 품질 |
| **PAE** | Predicted Aligned Error | 잔기 쌍 간 상대 위치 오차 |
| **DockQ** | interface quality (0-1) | >0.23 correct, >0.8 very high |

## Limitations

- 정적 구조만 예측 (dynamics 불가)
- 여러 seed 필요 — 단일 예측만으로는 최적 결과 보장 어려움
- Hallucination 가능: 신뢰도 낮은 예측도 confident하게 보일 수 있음
- Conformational coverage 제한: 일부 단백질의 열린/닫힌 상태 구분 어려움
- MSA depth가 낮으면 성능 저하 (특히 low-homology targets)

## Cross-References

- [[AlphaFold3]] — 도구 페이지
- [[AlphaFoldMultimer]] — AF3의 전신
- [[DiffusionModel]] — AF3의 핵심 아키텍처
- [[StructurePrediction]] — 구조 예측 개념
- [[Rosetta]] — 비교 대상 (에너지 기반 방법)
- [[DemisHassabis]] — Google DeepMind CEO, 공동 저자
- [[JohnJumper]] — corresponding author

## Source Citations
- [alphafold3_s41586-024-07487-w.pdf] — full paper
