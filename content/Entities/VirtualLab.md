---
aliases: [Virtual Lab, virtual-lab]
tags: [entity, tool, multi-agent]
sources: [The Virtual Lab_s41586-025-09442-9.pdf]
created: 2026-05-14
updated: 2026-05-14
---

# Virtual Lab

AI-human 협업 프레임워크로, LLM agent 팀이 학제간 연구를 수행한다. Stanford의 [[JamesZou]] 그룹에서 개발.

## Key Points

- **구성**: Human researcher + PI agent + Scientific Critic + domain-specific scientist agents
- **Agent 정의**: 각 agent는 Title, Expertise, Goal, Role로 specification
- **회의 방식**: Team meeting (broad, multi-agent) + Individual meeting (focused, single agent + critic)
- **Parallel meetings**: 같은 agenda를 high temperature로 5회 병렬 → low temperature로 merge
- **코드**: Python package `virtual-lab` v1.1.0 (GitHub: zou-group/virtual-lab)
- **기반 LLM**: Claude (Anthropic) — Opus, Sonnet, Haiku 사용

## Architecture

```
Human Researcher
    └── Principal Investigator (PI)
         ├── Scientific Critic
         ├── Immunologist
         ├── Machine Learning Specialist
         └── Computational Biologist
```

- PI가 회의 주재, 요약, 의사결정
- Scientific Critic이 모든 output에 비판적 피드백
- Human researcher는 high-level guidance만 제공 (전체 단어의 ~1-3%)

## Applications

현재는 nanobody design에 적용했지만, 어떤 학제간 연구에도 적용 가능:
- Agent 구성과 배경을 바꾸면 다른 도메인에 적용
- Schema(CLAUDE.md)에 해당하는 prompt가 각 agent를 정의

## Cross-References

- [[Swanson2025_VirtualLab|Virtual Lab 논문]]
- [[MultiAgentLLM]]
- [[JamesZou]]

## Source Citations
- [The Virtual Lab_s41586-025-09442-9.pdf] — full paper
