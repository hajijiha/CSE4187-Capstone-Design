# Project 1 · RAGstar

Linux 서버의 Out-of-Memory 장애 로그를 해석하는 온프레미스 RAG 진단 파이프라인입니다.
로컬 LLM, ChromaDB와 LangGraph를 결합해 파싱 → 분류 → 도구 실행·지식 검색 → 종합 진단을 수행합니다.

## 구조와 담당

```text
Streamlit 화면 → FastAPI Backend → AI 진단 파이프라인
                    ↓                  ↓
                 진단 이력         ChromaDB / Local LLM
```

팀 프로젝트에서 백엔드를 담당했습니다. FastAPI polling 서버와
진단 요청·결과 저장용 데이터 모델·스키마·API를 구현했습니다.

## 구현 저장소

| 구성 | 저장소 |
|---|---|
| AI 진단 서버 | [RAGstar-sogang/AI-server](https://github.com/RAGstar-sogang/AI-server) |
| Backend | [RAGstar-sogang/Backend-Server](https://github.com/RAGstar-sogang/Backend-Server) |
| Frontend | [RAGstar-sogang/Frontend-server](https://github.com/RAGstar-sogang/Frontend-server) |

## 시작하기

```bash
git clone https://github.com/RAGstar-sogang/Backend-Server.git
git clone https://github.com/RAGstar-sogang/AI-server.git
git clone https://github.com/RAGstar-sogang/Frontend-server.git
```

각 서버의 설치·환경 설정은 해당 저장소 README를 참고합니다.
AI 서버에는 로컬 모델과 지식 베이스가 필요합니다.

## 결과 자료

- [프로젝트 요약: 목표·범위·수행 결과](docs/project-summary.pdf)
- [ERD](docs/erd.pdf)
- [프로젝트 포스터](docs/poster.pdf)
- [개인 기술 보고서](docs/technical-report.docx)
- [팀 최종 발표](docs/presentation.pptx)
- [과목 강의계획서](../docs/syllabus.pdf)
