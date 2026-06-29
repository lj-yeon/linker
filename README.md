# LINKER 웹 시안 (나이스디앤비 외주)

(주)NICE디앤비 LINKER 서비스 **HTML/CSS 정적 시안** 프로젝트입니다.  
메인페이지 1종과 서브페이지 6종, 총 7개 HTML 파일로 구성됩니다.

---

## 프로젝트 개요

| 항목 | 내용 |
|------|------|
| **의뢰사** | (주)NICE디앤비 |
| **프로젝트** | LINKER 수출지원·바이어 발굴 서비스 웹 시안 |
| **형식** | HTML 단일 파일 (CSS 인라인, Vanilla JS) |
| **페이지 수** | 총 7종 (메인 1 + 서브 6) |

---

## 페이지 구성

### 메인페이지

| 파일 | 설명 |
|------|------|
| [index.html](./index.html) | BIG DATA / RPA / AI 히어로 슬라이더, 마케팅 서비스 소개, 6단계 서비스 프로세스 |

### 서브페이지 — 빅바이어 마케팅

| 파일 | 설명 |
|------|------|
| [sub-bigbuyer-finder.html](./sub-bigbuyer-finder.html) | 빅데이터 바이어 발굴 — 검색어·카테고리·국가 단계별 조건 설정 후 AI 발굴 실행 |
| [sub-bigbuyer-send.html](./sub-bigbuyer-send.html) | 마케팅 메시지 발송 — 발굴된 바이어 대상 이메일 마케팅 메시지 작성 및 발송 |
| [sub-bigbuyer-history.html](./sub-bigbuyer-history.html) | 임시저장내역 — 발송 전 저장된 마케팅 건 목록 조회 |

### 서브페이지 — 사업 참가신청

| 파일 | 설명 |
|------|------|
| [sub-apply.html](./sub-apply.html) | 사업 참가 신청 폼 — 사업명·품목·담당자 정보 입력 후 신청 제출 |
| [sub-apply-history.html](./sub-apply-history.html) | 신청내역 — 제출된 참가 신청 목록 조회 및 상태 확인 |
| [sub-apply-detail.html](./sub-apply-detail.html) | 신청 상세 — 신청 항목 읽기 전용 상세 보기 (신청내역에서 진입) |

---

## 주요 기능 및 UX

### 공통
- **스크롤 Sticky 헤더**: 스크롤 시 frosted glass 효과 (`backdrop-filter: blur`) 적용
- **Sticky 브레드크럼**: 스크롤 후 헤더 바로 아래 고정, 전체 너비 그림자 표시
- **모바일 페이지 타이틀**: 768px 이하에서 sticky 해제 (`position: static`)
- **모바일 햄버거 메뉴**: 슬라이드 애니메이션 (`transform: translateY`) 방식

### 빅데이터 바이어 발굴 페이지
- 검색어(최대 5개) / 카테고리(최대 3개) / 국가(최대 3개) 각각 최대 개수 제한 처리
- AI 바이어 발굴 클릭 시 **로딩 스피너 1.5초** 후 결과 패널 노출
- 오른쪽 사이드바에 선택된 조건 실시간 반영
- 브레드크럼에 "마케팅 메시지 발송" 노출하지 않음 (버튼으로만 진입)

### 반응형 (768px 이하)
- 브레드크럼: 홈 버튼 숨김, 각 셀렉트 `flex: 1` 균등 배분
- 폼 레이아웃: 라벨·필드 세로 배치
- 배너 padding·font-size 축소

---

## 파일 구조

```
linker/
├── index.html                  # 메인페이지
├── sub-bigbuyer-finder.html    # 빅데이터 바이어 발굴
├── sub-bigbuyer-send.html      # 마케팅 메시지 발송
├── sub-bigbuyer-history.html   # 임시저장내역
├── sub-apply.html              # 사업 참가 신청
├── sub-apply-history.html      # 신청내역
├── sub-apply-detail.html       # 신청 상세 (읽기 전용)
├── linker_eDM_des.d6ac8dbc.png # eDM 디자인 시안 이미지
├── linker_eDM_sample.pptx      # eDM 샘플 PPT
└── README.md
```

---

## 기술 스택

- HTML5, CSS3 (인라인 `<style>`)
- [Pretendard](https://github.com/orioncactus/pretendard) (CDN)
- [Font Awesome 6.5](https://fontawesome.com/) (CDN)
- Vanilla JavaScript (모바일 메뉴, 브레드크럼 sticky, 폼 유효성, 스피너 등)

---

## 로컬 실행

별도 빌드 없이 정적 HTML입니다.

```bash
python -m http.server 8080
# http://localhost:8080/index.html
```

---

## GitHub Pages 배포

1. GitHub 저장소 **Settings → Pages**
2. **Source**: Deploy from a branch
3. **Branch**: `main` / `/ (root)`
4. 저장 후 `https://lj-yeon.github.io/linker/` 접속

---

## 저작권

본 시안은 (주)NICE디앤비 외주 프로젝트용으로 제작되었습니다.  
푸터 및 로고 등 외부 리소스는 CTP·NICE디앤비 공식 자산 URL을 참조합니다.

© NICE D&B Co., Ltd.
