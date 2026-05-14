---
aliases: [ColabFold paper, ColabFold protocol]
tags: [paper, structure-prediction, protocol]
sources: [colabfold_s41596-024-01060-5.pdf]
created: 2026-05-14
updated: 2026-05-14
---

# Easy and accurate protein structure prediction using ColabFold

**Authors:** Gyuri Kim, Sewon Lee, Eli Levy Karin, Hyunbin Kim, ..., Martin Steinegger & Milot Mirdita
**Journal:** Nature Protocols, Vol 20, 2025
**DOI:** 10.1038/s41596-024-01060-5

## Summary

ColabFold는 AF2를 쉽게 사용할 수 있게 만든 오픈소스 도구로, Google Colab 노트북과 CLI를 제공한다. MMseqs2 기반 빠른 MSA 생성으로 AF2 대비 40-60배 빠른 속도를 달성하면서 유사한 정확도를 유지. 이 프로토콜 논문은 monomer prediction, complex prediction, conformational sampling의 3가지 시나리오를 가이드.

## Key Points

- **5개 노트북**: AlphaFold2.ipynb, RoseTTAFold2.ipynb, RoseTTAFold.ipynb, ESMFold.ipynb, OmegaFold.ipynb
- **MMseqs2** MSA server: UniRef + ColabFoldDB (>700M sequences) — 로컬 저장 불필요
- Monomer, complex, conformational sampling 3가지 사용 사례
- Google Colab에서 <2시간 내 실행 가능
- protocol.colabfold.com에서 무료 사용

## Cross-References

- [[Jumper2021_AlphaFold2|AF2 논문]]
- [[Baek2023_RoseTTAFold2|RF2 논문]]
- [[StructurePrediction]]

## Source Citations
- [colabfold_s41596-024-01060-5.pdf]
