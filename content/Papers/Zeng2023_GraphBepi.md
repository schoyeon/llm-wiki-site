---
aliases: [GraphBepi paper]
tags: [paper, epitope-prediction, B-cell, graph-neural-network]
sources: [graphbepi_btad187.pdf]
created: 2026-05-14
updated: 2026-05-14
---
# Identifying B-cell epitopes using AlphaFold2 predicted structures and pretrained language model
**Authors:** Yuansong Zeng, Zhuoyi Wei, Qianmu Yuan, Sheng Chen, Weijiang Yu, Yutong Lu, Jianzhao Gao & Yuedong Yang
**Journal:** Bioinformatics, 2023
**DOI:** 10.1093/bioinformatics/btad187
## Summary
GraphBepi는 AF2 예측 구조와 ESM-2 language model representation을 결합한 graph-based B-cell epitope 예측 모델. EGNN으로 structural information을 capture하고 BiLSTM으로 sequence long-range dependency를 학습. AUC/AUPR에서 기존 방법 대비 5.5%/44.0% 향상.
## Key Points
- AF2 predicted structure → protein graph → EGNN + BiLSTM
- ESM-2 pretrained embedding 활용
- 웹 서버: bio-web1.nscc-gz.cn/app/graphbepi
## Cross-References
- [[Hoie2024_DiscoTope3|DiscoTope-3.0]]
- [[Jumper2021_AlphaFold2|AF2]]
## Source Citations
- [graphbepi_btad187.pdf]
