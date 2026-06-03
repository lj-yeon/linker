# LINKER 웹 시안 (나이스디앤비 외주)

(주)NICE디앤비 LINKER 서비스 랜딩 페이지 **HTML/CSS 정적 시안** 프로젝트입니다.  
총 6가지 디자인 컨셉을 각각 독립 HTML 파일로 제공하며, GitHub Pages로 바로 미리볼 수 있습니다.

---

## 프로젝트 개요

| 항목 | 내용 |
|------|------|
| **의뢰사** | (주)NICE디앤비 |
| **프로젝트** | LINKER 수출지원·바이어 발굴 서비스 웹 시안 |
| **형식** | HTML 단일 파일 (CSS 인라인) |
| **시안 수** | 6종 + 목록 페이지 (`index.html`) |

---

## 시안 목록

| 파일 | 컨셉 | 특징 |
|------|------|------|
| [mockup-01.html](./mockup-01.html) | 공공·기관 클린 코퍼레이트 | 성장 막대그래프, 세계지도, stats 배너 |
| [mockup-02.html](./mockup-02.html) | 네이비 대시보드 | 도넛 차트, 지역별 데이터 리스트, 다크 히어로 |
| [mockup-03.html](./mockup-03.html) | 매거진·에디토리얼 | 태양계 오브 일러스트, 6단계 타임라인, 잡지형 카드 |
| [mockup-04.html](./mockup-04.html) | 공공·기관 모던 | 퀵메뉴 아이콘 바, SVG 도넛+데이터 테이블, 수평 카테고리 카드 |
| [mockup-05.html](./mockup-05.html) | 테크니컬 다크 | 네온 매트릭스 다이어그램, 지역 타일 그리드, 터미널 스캔 패널 |
| [mockup-06.html](./mockup-06.html) | 트렌디 SaaS | 플로팅 서비스 카드, SVG 도넛 범례, 그라디언트 피처 카드 |

메인 진입점: [index.html](./index.html) — 6개 시안 썸네일·설명·링크 목록

---

## 주요 섹션 구성 (공통)

각 시안은 아래 콘텐츠 블록을 동일하게 포함하되, **레이아웃·비주얼·컬러는 컨셉별로 차별화**되어 있습니다.

1. **헤더** — CTP 로고, GNB (수출바우처 컨설팅, 공지사항 등), 로그인/회원가입
2. **메인(히어로)** — 서비스 핵심 카피 및 CTA
3. **서비스 소개** — 6단계 프로세스 (빅데이터 발굴 → AI 추천 → 메시지 작성/발송 → 확인 → 답변)
4. **컨설팅 서비스** — 해외기업 신용조사, 글로벌 6개 지역 553,609,651건 데이터
5. **기업조회 서비스** — 금융기관 / 우량정보 / 등급정보 (D&B Rating, PAYDEX 등)
6. **푸터** — 개인정보처리방침, 이용약관, Family site 등

---

## 반응형·네비게이션

- **모바일** (~768px): 햄버거 메뉴, 1열 레이아웃, 가로 스크롤 방지
- **PC·태블릿** (768px+): 섹션 점프 네비게이션 (시안별 고유 디자인)
  - 01: 오른쪽 점 + 라벨
  - 02: 왼쪽 네이비 탭
  - 03: 오른쪽 에디토리얼 진행선
  - 04: 하단 아이콘 탭 바
  - 05: 오른쪽 네온 캡슐
  - 06: 하단 도트 pill

---

## 로컬 실행

별도 빌드 없이 정적 HTML입니다. 파일을 브라우저에서 열거나 로컬 서버로 실행하면 됩니다.

```bash
# Python 내장 서버 예시
python -m http.server 8080
# http://localhost:8080/index.html
```

---

## GitHub Pages 배포

1. GitHub 저장소 **Settings → Pages**
2. **Source**: Deploy from a branch
3. **Branch**: `main` / `/ (root)`
4. 저장 후 `https://<username>.github.io/linker/` 에서 `index.html` 접속

---

## 기술 스택

- HTML5, CSS3 (인라인 스타일)
- [Pretendard](https://github.com/orioncactus/pretendard) (CDN)
- [Font Awesome 6](https://fontawesome.com/) (CDN)
- Vanilla JavaScript (모바일 메뉴, 섹션 scrollspy)

---

## 파일 구조

```
linker/
├── index.html      # 시안 목록 (메인)
├── mockup-01.html  # 시안 1
├── mockup-02.html  # 시안 2
├── mockup-03.html  # 시안 3
├── mockup-04.html  # 시안 4
├── mockup-05.html  # 시안 5
├── mockup-06.html  # 시안 6
└── README.md
```

---

## 저작권

본 시안은 (주)NICE디앤비 외주 프로젝트용으로 제작되었습니다.  
푸터 및 로고 등 외부 리소스는 CTP·NICE디앤비 공식 자산 URL을 참조합니다.

© NICE D&B Co., Ltd.
