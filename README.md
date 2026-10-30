# 안녕하세요, 박윤후입니다 👋

**AI를 "그럴듯한 출력"이 아니라 _검증·보안·배포 가능한 시스템_으로 만드는 AI 엔지니어입니다.**
LLM 에이전트의 신뢰성, 인과추론 기반 데이터 분석, 의료 시계열 모델을 만들고, 평가 수치와 한계까지 문서에 공개합니다.

[![Portfolio](https://img.shields.io/badge/Portfolio-park--yunhu--portfolio-111111?style=flat-square&logo=vercel&logoColor=white)](https://park-yunhu-portfolio.vercel.app)
[![Gmail](https://img.shields.io/badge/Gmail-byunhu35@gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:byunhu35@gmail.com)

---

## 🎯 What I Do

- **신뢰할 수 있는 LLM 에이전트** — 근거 연결 검증, 사람 승인 지점, 실패 시 중단(fail-closed), 비용 상한
- **상관을 넘어 인과로** — PSM · 고정효과 · DiD로 "정말 효과가 있었는가"를 검증
- **의료 AI** — 결측 상태를 구분하는 ICU 패혈증 예측 모델, 응급 의사결정 시스템

---

## 🚀 Featured Projects

### 🤖 [algo-pipeline](https://github.com/YunhuPark/algo-pipeline) — 근거 검증형 LLM 에이전트
AI·테크 뉴스를 수집해 **출처 근거가 있는** 카드뉴스를 만들고 Instagram에 게시하는 자동화 에이전트.
수집 → 주장(claim) 추출 → 규칙 검증 → 의미 비평 → 렌더링 → 게시. 근거에 연결된 주장만 다음 단계로 넘어갑니다.
- 게시 시도를 호출 전에 DB에 먼저 기록, 자동 게시는 기본값 OFF, 검증 실패 시 중단
- `Python` `OpenAI` `FastAPI` `SQLite` `GitHub Actions` · [라이브 포트폴리오](https://algo-site-hazel.vercel.app)

### 🛡️ [devorch](https://github.com/YunhuPark/devorch) — AI 코딩 에이전트 통제·평가 도구
에이전트가 쓴 변경을 위험도 분석 → 독립 리뷰 → 임시 환경 테스트 → **사람 승인**을 거쳐야만 반영하는 MCP 기반 검문소.
- 1인 개발 · Python 모듈 63개 · 테스트 734개 · 서명된 감사 로그 · Docker 샌드박스
- 결함 주입 16케이스 + 공개 저장소 실제 결함 12개로 평가, **한계(실제 결함 5/12 탐지)까지 그대로 공개**
- `Python` `MCP` `Docker` `Anthropic / OpenAI / Gemini`

### 📊 [Medical_Insight_Lab](https://github.com/YunhuPark/Medical_Insight_Lab) — 상관에서 인과까지
한국 의료 유튜브 3,700여 개 영상으로 "공포 키워드 제목이 조회수를 높이는가"를 검증.
단순 비교 → 영상 나이 보정 → PSM → 채널 고정효과 → DiD. **직관과 달리 PSM 후 0.63배**로 낮았고, 채널 내에서는 불확실하다는 결과를 그대로 보고했습니다.
- `Python` `statsmodels` `scikit-learn` `SHAP` `Streamlit`

### 📈 [yt-growth-coach](https://github.com/YunhuPark/yt-growth-coach) — 기준선과 피드백 루프
채널 지표와 트렌드로 다음 영상 아이디어를 추천하고, 성과를 추적해 다음 추천에 반영하는 앱.
- 기준선 대비 "상위 몇 %" 비교, 표본 5개 미만이면 판단 보류, AI 점수를 실제 성과와 Spearman으로 검증
- `Next.js` `TypeScript` `Claude API` `FFmpeg`

### 🔎 [topic-ai](https://github.com/YunhuPark/topic-ai) — 이종 자료 통합 RAG
Notion · Slack · Drive · GitHub에 흩어진 지식을 통합 검색하고 요약·액션 아이템을 추출. **"검색은 공유해도 권한은 공유하지 않는다."**
- `FastAPI` `LangChain` `Chroma` `React`

### 🗺️ [tour-gap](https://github.com/YunhuPark/tour-gap) — 지역관광 의사결정 시스템
강원 18개 시군의 관광 수요·공급·체류 성과를 교차 검증. 독립 지표 검증과 108개 조합 민감도 분석.

---

## 🔬 Research

- [IMST-Mamba](https://github.com/YunhuPark/IMST-Mamba) — 결측을 미관측·최근·오래됨으로 구분하는 ICU 조기 패혈증 예측 모델 _(개인 연구, 미게재 초안)_
- [Medi-Matrix](https://github.com/YunhuPark/Medi-Matrix) · [golden-time](https://github.com/YunhuPark/golden-time) — 의료 영상·패혈증 예측 기반 응급도 산출, 실시간 응급실 안내

---

## 🛠️ Tech Stack

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)

![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=flat-square&logo=openai&logoColor=white)
![MCP](https://img.shields.io/badge/MCP-000000?style=flat-square)

![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white)

---

## 📐 How I Build

1. **근거 없는 주장은 통과시키지 않는다** — 규칙 검증 → 의미 비평 → 사람 승인
2. **불확실하면 결론 대신 보류한다** — 표본이 부족하면 판단을 내리지 않는다
3. **수치와 한계를 함께 공개한다** — 잘 안 된 결과도 README에 남긴다
