# ✨ 팀 프로젝트 - Study With Me

---

- **프로젝트 이름**: Study With Me
- **팀 이름**: 
- **프로젝트 목표**:  학습 및 일정 관리를 효율적으로 지원하는 학습플레너 개발 \
                    **스톱워치, 할 일 목록, AI 기반 로그 분석 기능, 개인별 학습 업적 로그 생성**을 통합하여 자바 스크립트 역량 강화
- **배포 링크**: 

--- 

## ⚙ 사용 기술

- **Frontend**
  
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-original.svg" alt="HTML5" width="40" height="40"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-original.svg" alt="CSS3" width="40" height="40"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg" alt="JavaScript" width="40" height="40"/>

- **협업 & 형상관리**

  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/git/git-original.svg" alt="Git" width="40" height="40"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/github/github-original.svg" alt="GitHub" width="40" height="40"/>
  <img src="https://www.svgrepo.com/show/353655/discord-icon.svg" alt="Discord" width="40" height="40"/>
---

| 역할   | 이름 | 담당 | 회고록 링크                                                                                                                                                                                       |
|--------|------|------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 팀장   | [고동현](https://github.com/rhehdgus8831) | 스톱워치 기능,명언 API 연동, GitHub 관리 및 PR 관리, README 작성,기본 | [고동현 회고록]()|
| 팀원   | [김경민](https://github.com/minee0505) | 할 일 추가 및 완료 상태를 관리하는 간단한 일정 관리 TodoList 기능 개발 | [김경민 회고록]() |
| 팀원   | [백승현](https://github.com/Sirosho) | 로컬 스토리지에 저장된 데이터 기반으로 개인별 학습 업적 로그 생성  | [백승현 회고록]()                                                                                                                                                                          |
| 팀원   | [송민재](https://github.com/songkey06) | Gemini API를 연동하여 사용자의 질문에 AI가 답변해주는 학습 보조 기능 개발, 프로젝트 발표 | [송민재 회고록]()                                                                                                                         |



---

## ✅ 주요 기능 요약

| 우선순위 | 기능명                   | 담당자 | 주요 기능 설명                                          |
|-----| --------------------- | --- | ------------------------------------------------- |
| Must Have | **스톱워치**              | 고동현 | 공부 시간 측정을 위한 스톱워치 기능 구현 및 누적 시간 저장(localStorage) |
| Must Have | **명언 표시**             | 고동현 | 학습 동기를 위한 명언 API 연동 및 랜덤 명언 출력 기능                 |
| Must Have | **할 일 목록 (TodoList)** | 김경민 | 할 일 추가/완료, 오늘·주간·완료 탭 구성, 체크박스 상태 관리,완료된 할일 갯수 저장(localStorage)            |
| Must Have | **학습 업적 로그**        | 백승현 | 공부 시간·할일·AI 질문 수 통합하여 로컬 스토리지 기반 학습 업적 기록 생성(업적 배지 시스템 구현)     |
| Must Have | **AI 학습 보조**          | 송민재 | Gemini API 연동을 통한 AI 질문/답변 기능 및 질문 로그 저장,질문 수량 갯수 저장(localStorage)          |



---

## 🗓️ 개발 일정

| 날짜 | 요일  | 내용                     |
| --- | --- | ---------------------- |
| 250623 | 월요일 | 주제 선정, Git & HTML,CSS 구조 세팅 |
| 250624 | 화요일 | 본격적인 기능 개발 시작        |
| 250625 | 수요일 | 기능 개발 계속               |
| 250626 | 목요일 | 모듈화, develop 브랜치 1차 병합, 1차 버그 픽스  |
| 250627 | 금요일 | develop 브랜치 2차 병합, 2차 버그 픽스      |
| 250628 | 토요일 | 개발 지속      |
| 250629 | 일요일 | 기능 마무리 및 테스트           |
| 250630 | 월요일 | 전체 버그 픽스 및 main 브랜치 최종 병합      |
| 250701 | 화요일 | PPT 제작, README 작성, 개인 회고록 작성      |
| 250702 | 수요일 | 최종 발표(송민재 발표)                  |

---

## 🛠️ Git 브랜치 전략


```
| * AiQuestion
| * playTime
| * toDoList
| * stopwatch
|/
* develop
|
* main
    
```

---

## 🧹 폴더 구조

```

HTML ─ index.html      # HTML 구조

/CSS
├── main.css         # 전체 스타일 설정 @import tag 용도
├── root.css         # 공용 컬러 디자인 분리
├── reset.css        # css 초기화 분리
├── stopwatch.css    # 스톱워치 디자인 스타일 분리
├── aiQuestion.css   # AI 디자인 스타일 분리
├── playTime.css     # 업적 기록 디자인 스타일 분리
└── list.css         # todolist 디자인 스타일 분리

/JS
  ├── app.js           # 최상위 진입점
  ├── stopwatch/       # 고동현 기능 모듈
  ├── todo/            # 김경민 기능 모듈
  ├── calendar/        # 백승현 기능 모듈
  └── ai/              # 송민재 기능 모듈

/assets
  └── images/          # 아이콘 및 이미지 등
```

---

## 📋 스크럼 및 협업 방식

* 매일 오후 개발 시작 전 **스크럼 회의**
* 주요 진행 상황 및 **이슈 GitHub에 등록**
* `main → develop → feature` 브랜치 전략 유지
* 각자 담당 기능을 모듈화해서 반영
* 팀 전체 CSS 통일 (공통 `main.css` + 개념 CSS)

---
## 📅 진행 로그

### 🗓 2025년 6월 23일 회의

| 항목            | 내용 |
|-----------------|------|
| 기능 개발 주제 | ToDoList  |
| 선정 이유         | 기존에 학습했던 JS 기술 기반을 다양하게 사용할 수 있어 선정함 |
| 오늘의 To Do      | 아래 참고 |

**To Do**
- HTML 및 CSS 구조 작업
- 브랜치 전략 및 파일 구조 통일

---

### 🗓 2025년 6월 24일 회의

| 항목            | 내용 |
|-----------------|------|
| 주요 논의 | 작업 시작 전 이슈 등록 및 JS 개발 작업  |
| 오늘의 To Do      | 아래 참고 |

**To Do**


- **고동현**: README 작성, 스톱워치 구현
- **김경민**: JS 투두리스트 기능 구현
- **백승현**: 유저 업적 기록 그래프 랜더링 CSS
- **송민재**: Gemini API 로 호출해서 로그 받기

---
### 🗓 2025년 6월 25일 회의

| 항목            | 내용 |
|-----------------|------|
| 주요 논의 | 24일 작업 내용 브리핑 및 1차 병합하면서 충돌해결 후 코드리뷰 진행  |
| 오늘의 To Do      | 아래 참고 |

**To Do**
- ```app.js``` 내 JS 모듈을 ```import``` 방식으로 정리
- 금일 작업 내용 이슈 등록

- **고동현**: README 작성, 오늘의 명언 API 연동 및 랜더링
- **김경민**: ToDoList 기능에 Drag & Drop 기능 구현
- **백승현**: 유저 업적 기록 시각화를 위한 그래프 스타일 및 CSS 작업 
- **송민재**:  Gemini API에서 받은 JSON 응답 문자열을 각 항목별로 구분하여 렌더링할 수 있도록 구현 \
줄바꿈 처리 및 Key/Value 형식이 시각적으로 잘 보이도록 개선 예정
---

### 🗓 2025년 6월 26일 회의

| 항목            | 내용 |
|-----------------|------|
| 주요 논의 |   |
| 오늘의 To Do      | 아래 참고 |

**To Do**


- **고동현**: 
- **김경민**: 
- **백승현**: 
- **송민재**: 
---

### 🗓 2025년 6월 27일 회의

| 항목            | 내용 |
|-----------------|------|
| 주요 논의 |   |
| 오늘의 To Do      | 아래 참고 |

**To Do**


- **고동현**: 
- **김경민**: 
- **백승현**: 
- **송민재**: 
---

### 🗓 2025년 6월 30일 회의

| 항목            | 내용 |
|-----------------|------|
| 주요 논의 |   |
| 오늘의 To Do      | 아래 참고 |

**To Do**


- **고동현**: 
- **김경민**: 
- **백승현**: 
- **송민재**: 
---

### 🗓 2025년 7월 1일 회의

| 항목            | 내용 |
|-----------------|------|
| 주요 논의 |   |
| 오늘의 To Do      | 아래 참고 |

**To Do**


- **고동현**: 
- **김경민**: 
- **백승현**: 
- **송민재**: 
---

---
## ⚠️ Trouble Shooting

### 1.

- **문제**:
- **원인**:
- **해결**:
- **협업 포인트**:
- 
---

### 2

- **문제**:
- **원인**:
- **해결**:
- **협업 포인트**:

---

## 저작권

- 명언 API  
  ⤷ 출처: [korean-advice-open-api](https://github.com/gwongibeom/korean-advice-open-api)

- AI 응답 기능  
  ⤷ 본 프로젝트는 Google에서 제공하는 [Gemini API](https://ai.google.dev/)를 기반으로 AI 응답을 제공합니다.

