---
aliases: [diffusion model, denoising diffusion, diffusion-based generation]
tags: [concept, deep-learning, generative-model]
sources: [alphafold3_s41586-024-07487-w.pdf]
created: 2026-05-14
updated: 2026-05-14
---

# Diffusion Model

노이즈를 점진적으로 제거하여 데이터를 생성하는 생성 모델. 이미지 생성(DALL-E, Stable Diffusion)에서 시작하여, 단백질 구조 예측/설계에도 핵심 역할.

## Key Points

- **원리**: 데이터에 노이즈 추가 (forward) → 노이즈 제거 학습 (reverse) → 새 데이터 생성
- **장점**: 분포의 다양성을 잘 포착, multiple samples로 다양한 구조 생성 가능
- **구조 예측에서**: 원자 좌표에 직접 적용 — rotational frame 불필요

## 구조 생물학에서의 활용

| 도구 | 용도 | diffusion 적용 |
|-----|------|-------------|
| [[AlphaFold3]] | 구조 예측 | 원자 좌표 denoising |
| RFdiffusion | 단백질 설계 | backbone 생성 |
| DiffDock | 도킹 | 리간드 pose 생성 |
| Chroma | 단백질 설계 | 전체 구조 생성 |

## Cross-References

- [[Abramson2024_AlphaFold3|AF3 논문]]
- [[AlphaFold3]]
- [[StructurePrediction]]

## Source Citations
- [alphafold3_s41586-024-07487-w.pdf]
