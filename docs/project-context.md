# 프로젝트 컨텍스트

> tide 워크플로우(`/tide:milestone`·`/tide:impl`)가 매번 재조사하지 않고 참조하는 구조 문서.
> 한 줄 설명: **자기소개를 위한 GitHub Pages 소스 — 개발 경력 및 AI 활용 능력 소개**

---

## 스택 · 언어 · 주요 의존성

- **유형**: 순수 정적 사이트 (빌드 단계 없음, 프레임워크·외부 라이브러리 비종속)
- **언어**: HTML · CSS · 바닐라 JavaScript
- **콘텐츠 언어**: 한국어
- **배포**: GitHub Pages — `master` 브랜치 루트(`/`)에서 직접 서빙 (URL: https://jongh.github.io)
- **Jekyll**: `.nojekyll`로 비활성화 (기존 `_posts/`·`_pages/` 잔류하나 무해)
- **의존성·패키지 매니저**: 없음 (버전 파일 부재)

---

## 최상위 디렉터리 구조

| 경로 | 역할 |
|------|------|
| `index.html` | 단일 페이지 (7개 섹션 + sticky 네비, 베이지 테마) |
| `style.css` | 베이지 테마·반응형·애니메이션 |
| `main.js` | IntersectionObserver 기반 스크롤 fade-in |
| `favicon.png` | 파비콘 (얼굴 크롭 180×180) |
| `.nojekyll` | Jekyll 빌드 비활성화 |
| `assets/image/` | 프로필 일러스트·아바타·OG 썸네일 이미지 |
| `assets/resume/` | 웹 공개용 이력서 PDF (전화번호 제거·고객사명 일반화) |
| `docs/` | 설계·규약 문서 (ia-spec, copy-draft, conventions, milestones/, reports/) |
| `.docs/` | 내부 작업 문서 (`.gitignore`로 커밋 제외) |
| `_posts/` · `_pages/` | 기존 Jekyll 잔류 디렉터리 (미사용) |

---

## 진입점 · 빌드 / 테스트 실행 방법

- **진입점**: `index.html` (단일 페이지)
- **빌드**: 없음 — 정적 파일 그대로 서빙
- **로컬 미리보기**: 임의 정적 서버로 확인 (예: `python -m http.server`) 또는 `index.html` 직접 열기
- **테스트**: 자동화 테스트 프레임워크 없음 — 브라우저 수동 확인 (확인 필요: 추후 도입 여부)
- **배포**: `master` 브랜치 push 시 GitHub Pages 자동 반영

---

## 핵심 도메인 개념 · 용어

- **핵심 원칙**: 특정 언어/프레임워크/DB/제품명을 "역량"으로 소개하지 않는다. 항상
  "AI를 어떻게 다루는가"라는 **방법론 관점**으로 추상화한다.
- **페이지 구조 (7개 섹션)**: `#hero` · `#stats`(숫자로 보는 경력) · `#about`(자기소개) ·
  `#work-history`(업무 이력) · `#domains`(도메인·산업 경험 맵) · `#key-projects`(주요 업무) ·
  `#ai-strengths`(AI 활용 방법론) · `#workflow`(AI 협업 방식) · `#contact`(연락처/푸터).
- **소개하는 AI 활용 방법론 7가지**: ①컨텍스트 엔지니어링 ②작업 분해 ③역할 분업(오케스트레이션)
  ④검증·승인 게이트 ⑤검증 루프 ⑥의사결정 기록 ⑦재사용 자산화.
- **작업 페르소나 4종**: 🏛️ Architect(구조 설계) · ✍️ Writer(카피) · 🔨 Implementer(구현) ·
  🔍 Reviewer(비판적 검토).
- **보안 규약**: 모든 콘텐츠에서 고객사·협업처 실명 제거 → 산업/도메인 일반 표현으로 대체.
- **이름 표기**: 전 페이지 **김종현**으로 통일.

> 상세 배경·결정 이력은 루트 `CLAUDE.md`가 단일 원본이다.
