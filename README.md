# LINKER 웹 시안 (나이스디앤비 외주)

(주)NICE디앤비 LINKER 서비스 **HTML/CSS 정적 시안** 프로젝트입니다.  
메인페이지 시안 3종과 서브페이지 시안 4종, 총 7종을 각각 독립 HTML 파일로 제공합니다.

---

## 프로젝트 개요

| 항목 | 내용 |
|------|------|
| **의뢰사** | (주)NICE디앤비 |
| **프로젝트** | LINKER 수출지원·바이어 발굴 서비스 웹 시안 |
| **형식** | HTML 단일 파일 (CSS 인라인) |
| **시안 수** | 7종 (메인 3종 + 서브 4종) + 목록 페이지 (`index.html`) |

---

## 시안 목록

### 메인페이지 시안 (3종)

| 파일 | 컨셉 | 기획 의도 |
|------|------|-----------|
| [mockup-01.html](./mockup-01.html) | 5억 건+ 글로벌 기업 빅데이터 | 데이터 규모를 지구본 그래픽으로 시각화, 첫인상 임팩트 중심 |
| [mockup-02.html](./mockup-02.html) | 전통 클래식 공공기관 스타일 | 공공기관 사용자에게 익숙한 클래식 레이아웃으로 신뢰감·안정감 우선 |
| [mockup-03.html](./mockup-03.html) | 지자체 산하기관 스타일 | 지자체·산하기관 색채 체계 차용, 기관 협력 맥락에서 친화성 강조 |

### 서브페이지 시안 (4종)

#### 빅바이어마케팅

| 파일 | 컨셉 | 기획 의도 |
|------|------|-----------|
| [sub-bigbuyer-01.html](./sub-bigbuyer-01.html) | 버전 1 · 클래식 수직 스택 | 검색 중심 태스크에 집중, 조건 필터를 한 화면에 모아 효율성 극대화 |
| [sub-bigbuyer-02.html](./sub-bigbuyer-02.html) | 버전 2 · 단계별 가이드 | 단계별 가이드로 처음 사용자도 이탈 없이 완료 유도 (위자드 UX) |

#### 전시회 참가신청

| 파일 | 컨셉 | 기획 의도 |
|------|------|-----------|
| [sub-apply.html](./sub-apply.html) | 참가신청 폼 | 배너 스타일을 변경하고, 내용은 기존 LINKER 스타일을 유지하며 참가신청에 필요한 항목으로 구성 |
| [sub-apply-history.html](./sub-apply-history.html) | 신청내역 검색 | 배너 스타일을 변경하고, 내용은 기존 LINKER 스타일을 유지하며 신청내역 조회에 필요한 항목으로 구성 |

메인 진입점: [index.html](./index.html) — 7개 시안 썸네일·기획의도·링크 목록

---

## 반응형·네비게이션

- **모바일** (~768px): 햄버거 메뉴, 1열 레이아웃, 가로 스크롤 방지
- **서브페이지 브레드크럼**: 스크롤 시 헤더 하단에 sticky 고정, 모바일에서 홈 숨김 및 전체 너비 확장
- **브레드크럼 내비게이션**: 모든 서브페이지 간 이동 가능 (빅바이어마케팅 V1·V2 / 전시회 참가신청·신청내역)
- **PC·태블릿** (768px+): GNB 노출, 브레드크럼 좌측 정렬

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
4. 저장 후 `https://lj-yeon.github.io/linker/` 에서 `index.html` 접속

---

## 기술 스택

- HTML5, CSS3 (인라인 스타일)
- [Pretendard](https://github.com/orioncactus/pretendard) (CDN)
- [Font Awesome 6](https://fontawesome.com/) (CDN)
- Vanilla JavaScript (모바일 메뉴, 브레드크럼 내비게이션, 폼 유효성 검사)

---

## 파일 구조

```
linker/
├── index.html              # 시안 목록 (메인)
├── mockup-01.html          # 메인 시안 1 — 빅데이터 글로브 히어로
├── mockup-02.html          # 메인 시안 2 — 전통 클래식 공공기관
├── mockup-03.html          # 메인 시안 3 — 지자체 산하기관
├── sub-bigbuyer-01.html    # 서브 — 빅바이어마케팅 V1 (클래식 검색)
├── sub-bigbuyer-02.html    # 서브 — 빅바이어마케팅 V2 (단계별 가이드)
├── sub-apply.html          # 서브 — 전시회 참가신청 폼
├── sub-apply-history.html  # 서브 — 신청내역 검색
└── README.md
```

---

## 저작권

본 시안은 (주)NICE디앤비 외주 프로젝트용으로 제작되었습니다.  
푸터 및 로고 등 외부 리소스는 CTP·NICE디앤비 공식 자산 URL을 참조합니다.

© NICE D&B Co., Ltd.
