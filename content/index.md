---
title: LLM Wiki
---

# LLM Wiki

Karpathy의 [LLM Wiki](https://gist.github.com/karpathy/442a6bf555914893e9891c11519de94f) 컨셉 기반 개인 지식 위키.

**소스를 넣으면 LLM이 정리/연결/유지보수를 전부 합니다.**

## Upload & Browse

- **[+ 논문 업로드하기](https://github.com/schoyeon/llm-wiki-site/upload/main/content)** — PDF를 드래그앤드롭으로 업로드
- [[MasterIndex|Master Index]] — 전체 페이지 목록
- [[IngestQueue|Ingest Queue]] — 처리 대기열

## Sections

| 폴더 | 내용 |
|------|------|
| **Papers/** | 논문/기사 요약 |
| **Entities/** | 인물, 조직, 도구, 모델 |
| **Concepts/** | 개념, 방법론, 이론 |
| **Topics/** | 주제별 종합 |

## How it works

1. `_sources/`에 원본 자료를 넣는다
2. Claude에게 ingest를 요청한다
3. 자동으로 요약, 엔티티 추출, 크로스레퍼런스 생성
4. 이 위키가 점점 풍부해진다
