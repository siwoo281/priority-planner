# Priority Planner (아이젠하워 매트릭스)

아이젠하워 매트릭스를 기반으로 한 모던한 작업 관리 웹 애플리케이션입니다. 중요도와 긴급도에 따라 작업을 4개의 분면으로 분류하여 우선순위를 효율적으로 관리할 수 있습니다.

![아이젠하워 매트릭스](https://img.shields.io/badge/Eisenhower-Matrix-blue)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)

## 📋 주요 기능

### ✅ 작업 관리
- **4분면 분류**: 중요도와 긴급도에 따른 작업 분류
  - **Q1**: 중요 & 긴급 (즉시 처리)
  - **Q2**: 중요 & 긴급하지 않음 (계획 수립)
  - **Q3**: 중요하지 않음 & 긴급 (위임 가능)
  - **Q4**: 중요하지 않음 & 긴급하지 않음 (제거 고려)

### 🎯 핵심 기능
- ✨ **드래그 앤 드롭**: 작업을 분면 간에 자유롭게 이동
- ✏️ **작업 편집**: 작업 내용, 카테고리, 마감일, 메모 수정
- ✅ **완료 관리**: 작업 완료 토글 및 완료된 작업 목록
- 💾 **로컬 저장**: 브라우저 로컬 스토리지에 자동 저장
- 📅 **마감일 관리**: 마감일 설정 및 지난 마감일 시각적 표시
- 🏷️ **카테고리 분류**: 업무, 학습, 개인, 프로젝트, 기타
- 📝 **메모 기능**: 작업별 상세 메모 추가
- 🔔 **토스트 알림**: 작업 추가/수정/삭제 시 피드백

### 🎨 UI/UX
- 모던하고 깔끔한 디자인
- 반응형 레이아웃 (모바일 지원)
- 직관적인 인터페이스
- 부드러운 애니메이션 효과
- 접근성 고려 (ARIA 속성, 키보드 네비게이션)

## 🚀 사용 방법

### 온라인 버전
GitHub Pages를 통해 바로 사용할 수 있습니다. (설정 필요)

### 로컬 실행
1. 저장소 클론
```bash
git clone https://github.com/siwoo281/priority-planner.git
cd priority-planner
```

2. `index.html` 파일을 브라우저로 열기
```bash
# macOS
open index.html

# Windows
start index.html

# Linux
xdg-open index.html
```

또는 로컬 서버 실행:
```bash
# Python 3
python -m http.server 8000

# Node.js (http-server 설치 필요)
npx http-server
```

3. 브라우저에서 `http://localhost:8000` 접속

## 📖 사용 가이드

### 작업 추가
1. 상단 입력창에 작업 내용 입력
2. **긴급함**, **중요함** 체크박스 선택
3. 선택적으로 카테고리, 마감일, 메모 입력
4. **작업 추가** 버튼 클릭

### 작업 관리
- **편집**: 작업 카드의 "편집" 버튼 클릭
- **완료**: 작업 카드 왼쪽의 체크박스 클릭
- **삭제**: 작업 카드의 "삭제" 버튼 클릭
- **이동**: 작업 카드를 드래그하여 다른 분면으로 이동

### 완료된 작업
- 하단의 "완료된 작업" 섹션에서 확인
- 완료된 작업은 복원 또는 삭제 가능
- "완료 항목 비우기" 버튼으로 일괄 삭제

## 🛠️ 기술 스택

- **HTML5**: 시맨틱 마크업
- **CSS3**: CSS Grid, Flexbox, CSS Variables
- **JavaScript (ES6+)**: 
  - 로컬 스토리지 API
  - 드래그 앤 드롭 API
  - DOM 조작

## 📁 프로젝트 구조

```
priority-planner/
├── index.html          # 단일 파일 애플리케이션
└── README.md          # 프로젝트 문서
```

모든 코드는 단일 HTML 파일에 포함되어 있어 배포가 간편합니다.

## 🌟 특징

- **서버리스**: 별도의 백엔드 서버 불필요
- **오프라인 지원**: 로컬 스토리지로 오프라인에서도 사용 가능
- **빠른 로딩**: 단일 파일로 구성되어 로딩 속도 빠름
- **프라이버시**: 모든 데이터가 브라우저에 저장되어 완전히 프라이빗

## 📝 아이젠하워 매트릭스란?

아이젠하워 매트릭스는 미국 제34대 대통령 드와이트 D. 아이젠하워의 시간 관리 원칙을 기반으로 한 우선순위 결정 도구입니다. 작업을 다음 4가지로 분류합니다:

1. **중요하고 긴급한 일**: 즉시 처리해야 할 일
2. **중요하지만 긴급하지 않은 일**: 계획을 세워 처리할 일
3. **중요하지 않지만 긴급한 일**: 다른 사람에게 위임하거나 최소한의 시간으로 처리할 일
4. **중요하지도 긴급하지도 않은 일**: 나중에 하거나 제거해야 할 일

## 🔄 업데이트 이력

### v1.0.0
- 초기 버전 릴리스
- 4분면 작업 분류
- 드래그 앤 드롭 기능
- 작업 편집/삭제/완료 기능
- 로컬 스토리지 저장
- 카테고리, 마감일, 메모 기능
- 완료된 작업 관리

## 🤝 기여하기

버그 리포트, 기능 제안, Pull Request를 환영합니다!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 라이선스

이 프로젝트는 MIT 라이선스 하에 배포됩니다. 자유롭게 사용, 수정, 배포할 수 있습니다.

## 📧 연락처

프로젝트 관련 문의사항이 있으시면 이슈를 등록해 주세요.

---

⭐ 이 프로젝트가 도움이 되셨다면 Star를 눌러주세요!

