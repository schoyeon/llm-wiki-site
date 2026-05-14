---
aliases: [RFAntibody paper]
tags: [paper, antibody, protein-design, diffusion]
sources: [rfantibody_s41586-025-09721-5.pdf]
created: 2026-05-14
updated: 2026-05-14
---

# Atomically accurate de novo design of antibodies with RFdiffusion

**Authors:** Nathaniel R. Bennett, Joseph L. Watson, Robert J. Ragotte, Andrew J. Borst, ..., David Baker
**Journal:** Nature, 2025
**DOI:** 10.1038/s41586-025-09721-5

## Summary

RFdiffusion 네트워크를 fine-tuning하여 epitope-specific VHH, scFv, full antibody를 de novo 설계하는 방법. 사용자 지정 epitope에 결합하는 항체의 CDR 루프 6개 모두를 원자 수준 정확도로 설계. 4개 disease-relevant epitope에 대해 실험 검증, Cryo-EM으로 binding pose 확인. OrthoRep으로 affinity maturation시 nanomolar~tens of nanomolar binding affinity 달성.

## Key Points

- RFdiffusion을 antibody structure에 fine-tuning (CDR H3 + framework)
- AF2로 RF2 format의 validation → 구조 필터링
- 4개 타겟 (인플루엔자 HA, C. difficile TcdB, PHOX2B peptide-MHC 등) 실험 검증
- Cryo-EM으로 원자 수준 정확도 확인
- Initial Kd: tens~hundreds nM → OrthoRep maturation → single-digit nM

## Cross-References

- [[Watson2023_RFdiffusion|RFdiffusion]]
- [[Dauparas2022_ProteinMPNN|ProteinMPNN]]
- [[Nanobody]]
- [[DiffusionModel]]

## Source Citations
- [rfantibody_s41586-025-09721-5.pdf]
