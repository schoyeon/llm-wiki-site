---
aliases: [Getting Started]
tags: [meta]
created: 2026-05-14
updated: 2026-05-14
---

# LLM Wiki — Quick Start

Karpathy의 LLM Wiki 컨셉 기반 개인 지식 위키.
**당신은 소스를 넣고 질문만 하면 됩니다. LLM이 정리/연결/유지보수를 전부 합니다.**

## 구조

| 폴더 | 역할 |
|------|------|
| `_sources/` | 원본 자료 (PDF, 논문, 기사) — 수정 금지 |
| `Index/` | 마스터 인덱스, MOC |
| `Papers/` | 논문/기사 요약 페이지 |
| `Entities/` | 인물, 조직, 도구, 모델 |
| `Concepts/` | 개념, 방법론, 이론 |
| `Topics/` | 주제별 종합 페이지 |
| `_logs/` | 작업 로그 |

## 사용법

### 1. 소스 추가 (Ingest)
```bash
# 터미널에서:
cd ~/Documents/LLM-Wiki
./_scripts/ingest.sh ~/Downloads/some_paper.pdf

# 또는 직접 _sources/ 폴더에 파일을 넣어도 됩니다
```

### 2. Claude에게 처리 요청
```
cd ~/Documents/LLM-Wiki
claude

# Claude에게 말하기:
"_sources/some_paper.pdf를 ingest 해줘"
```

Claude가 자동으로:
- 요약 페이지 생성
- 엔티티/개념 페이지 생성 또는 업데이트
- 크로스 레퍼런스 연결
- 인덱스 업데이트
- 로그 기록

### 3. 질문하기 (Query)
```
"Transformer의 attention mechanism에 대해 위키에서 찾아줘"
"RFdiffusion과 ProteinMPNN의 관계를 정리해줘"
```

### 4. 위키 점검 (Lint)
```
"위키 lint 해줘"
```
→ 고아 페이지, 깨진 링크, 모순점, 오래된 페이지 등을 점검

### 5. 재구성 (Reorganize)
```
"위키 reorg 해줘"
```
→ 중복 합치기, 큰 페이지 분할, 태그 정리

## Tips
- Obsidian에서 Graph View를 켜면 지식 맵이 시각화됩니다
- `_sources/`에는 무엇이든 넣을 수 있습니다 (PDF, 웹페이지, 메모, 코드)
- 질문의 답이 좋으면 그 자체가 새 위키 페이지가 됩니다 — 지식이 복리로 쌓입니다
