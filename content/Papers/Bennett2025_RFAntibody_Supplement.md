---
aliases: [RFAntibody supplementary, RFAntibody methods]
tags: [paper, antibody, protein-design, diffusion, supplementary]
sources: [rfantibody_detail_41586_2025_9721_MOESM1_ESM.pdf]
created: 2026-05-14
updated: 2026-05-14
---

# RFAntibody — Supplementary Information

**Parent paper:** [[Bennett2025_RFAntibody|RFAntibody 본문]]

## Contents Overview (70+ pages)

### Part I: Supplementary Figures (SI Fig 1-16)
- Design campaign 결과, binding assay, cryo-EM 구조 상세, CDR loop 분석 등

### Part II: RFdiffusion & RoseTTAFold2 Training Methods

#### Training Datasets (Section 1)
- **SAbDab**: antibody 구조 데이터베이스
- **TCR/MHC-Peptide**: crystal + AF2 predicted structures
- **Loop-mediated interactions**: PDB에서 loop 기반 상호작용 추출

#### Vanilla RFdiffusion Review (Section 2)
- Noising/denoising, losses, structure self-conditioning
- Vanilla RFdiffusion은 antibody complex에서 잘 작동하지 않음 → fine-tuning 필요

#### RFdiffusion for Antibody Design (Section 3)
- **Datasets**: SAbDab + TCR/MHC + loop interactions
- **Template provision**: target epitope 정보 제공 방법
- **Sequence self-conditioning**: CDR 서열 예측을 self-conditioning에 활용
- **Interface hotspots**: target residue 지정 방법
- **Training details**: training schedule, hyperparameters

#### RoseTTAFold2 Review (Section 4)
- RF2 auxiliary heads: pLDDT, PAE, **pBind** (결합 예측 head)
- pBind: 설계된 antibody-antigen complex의 결합 가능성 예측

#### Fine-Tuning RF2 for Ab Complex Prediction (Section 5)
- **Updated pBind head**: 결합 예측 성능 향상
- **Hotspot information**: RF2에 hotspot residue 정보 전달
- **Target structure provision**: 다양한 cropping 전략
- **Negative examples**: non-binding pair 생성 방법
- **CDR loop swapping**: data augmentation
- **De novo miniprotein binder set**: 추가 학습 데이터

### Part III: Computational Methods (Section 6)

| 단계 | 방법 | 상세 |
|------|------|------|
| Backbone 생성 | RFdiffusion (fine-tuned) | VHH/scFv CDR 생성 |
| 서열 설계 | ProteinMPNN | Ab-specific settings |
| 구조 검증 | RoseTTAFold2 | True/decoy discrimination |
| Monomer 검증 | RF2 / IgFold | Ab monomer fold 확인 |
| Interface 분석 | designed vs native interface 비교 | RMSD, contact overlap |
| Humanness 평가 | VHH/scFv structural similarity to PDB | human germline 유사도 |

#### VHH Design Campaigns (Section 6.8)
- HA (인플루엔자), TcdB (C. difficile) 타겟
- Hotspot residue selection → RFdiffusion → ProteinMPNN → RF2 필터링

#### scFv Design Campaigns (Section 6.9-6.10)
- TcdB scFv, Phox2b peptide-MHC scFv
- Heavy + light chain 조합 설계

## Cross-References

- [[Bennett2025_RFAntibody|RFAntibody 본문]]
- [[Watson2023_RFdiffusion|RFdiffusion]]
- [[Baek2023_RoseTTAFold2|RoseTTAFold2]]
- [[Dauparas2022_ProteinMPNN|ProteinMPNN]]
- [[Nanobody]]
- [[DiffusionModel]]

## Source Citations
- [rfantibody_detail_41586_2025_9721_MOESM1_ESM.pdf]
