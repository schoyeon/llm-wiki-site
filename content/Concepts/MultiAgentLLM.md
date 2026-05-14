---
aliases: [multi-agent LLM, multi-agent system, LLM agents]
tags: [concept, LLM, AI]
sources: [The Virtual Lab_s41586-025-09442-9.pdf]
created: 2026-05-14
updated: 2026-05-14
---

# Multi-Agent LLM Systems

여러 LLM agent가 각자 역할을 맡아 협업하는 시스템. 단일 LLM 대비 다양한 관점에서의 reasoning과 자체 비판이 가능.

## Key Points

- 각 agent에 Title, Expertise, Goal, Role을 부여하여 persona 분리
- Chain-of-thought와 유사하게, 서로 다른 agent 관점이 더 깊은 reasoning을 유도
- Scientific Critic 역할이 hallucination과 bias를 줄이는 데 핵심
- Parallel meeting (high temp) → merge (low temp) 패턴으로 robustness 확보

## 관련 시스템

- [[VirtualLab]] — 학제간 연구용 multi-agent
- AI Scientist (Lu et al., 2024) — open-ended scientific discovery
- ChatDev, MetaGPT 등 — software engineering용 multi-agent

## Cross-References

- [[Swanson2025_VirtualLab|Virtual Lab 논문]]
- [[VirtualLab]]

## Source Citations
- [The Virtual Lab_s41586-025-09442-9.pdf]
