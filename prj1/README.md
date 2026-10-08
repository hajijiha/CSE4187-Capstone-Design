# Project 1 · RAGstar

Linux 서버의 Out-of-Memory 장애 로그를 해석하는 온프레미스 RAG 진단 파이프라인입니다.
로컬 LLM, ChromaDB와 LangGraph를 결합해 파싱 → 분류 → 도구 실행·지식 검색 → 종합 진단을 수행합니다.

## 구조와 담당

```text
Streamlit 화면 → FastAPI Backend → AI 진단 파이프라인
                    ↓                  ↓
                 진단 이력         ChromaDB / Local LLM
```

팀 프로젝트이며, 하지훈의 백엔드 작업 이력에는 FastAPI polling 서버와
진단 요청·결과 저장을 위한 데이터 모델·스키마·API가 포함되어 있습니다.
이 저장소는 프로젝트 소개와 보고서 중심으로 정리하고 실제 코드는 팀 원본으로 연결합니다.

## 원본 저장소

| 구성 | 원본 |
|---|---|
| AI 진단 서버 | [RAGstar-sogang/AI-server](https://github.com/RAGstar-sogang/AI-server) |
| Backend | [RAGstar-sogang/Backend-Server](https://github.com/RAGstar-sogang/Backend-Server) |
| Frontend | [RAGstar-sogang/Frontend-server](https://github.com/RAGstar-sogang/Frontend-server) |

과거 로컬 체크아웃에는 `Web-server`라는 이름의 remote도 있으므로 현재 링크는
GitHub 계정에서 확인한 저장소 이름으로 기록했습니다.

## 시작하기

```bash
git clone https://github.com/RAGstar-sogang/Backend-Server.git
git clone https://github.com/RAGstar-sogang/AI-server.git
git clone https://github.com/RAGstar-sogang/Frontend-server.git
```

각 서버의 의존성, 로컬 모델·DB와 환경 변수 설정은 해당 팀 저장소 README를 따릅니다.
AI 서버에는 모델·지식 베이스 등의 별도 자원이 필요하므로 이 소개 저장소만으로
전체 시스템을 구동할 수 있는 것으로 표시하지 않습니다.

## 결과 자료

- [ERD](docs/erd.pdf)
- [프로젝트 포스터](docs/poster.pdf)
- [개인 기술 보고서](docs/technical-report.docx)
- [팀 최종 발표](docs/presentation.pptx)
- [과목 강의계획서](../docs/syllabus.pdf)

2026-1학기 강의계획서의 공식 과목코드는 `CSE4187`입니다.
