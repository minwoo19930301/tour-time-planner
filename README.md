# Tour Time Planner - Timeline Scheduler

[![Live Demo](https://img.shields.io/badge/Live%20Demo-GitHub%20Pages-brightgreen?style=for-the-badge&logo=github)](https://minwoo19930301.github.io/tour-time-planner/)


시간표 형태로 여행 일정을 짜고, 링크 하나로 그대로 공유할 수 있는 정적 웹앱입니다. 모바일 터치 편집과 드래그 이동까지 지원해서 여행 일정표를 빠르게 정리하기 좋습니다.

## 링크

- 서비스: [Tour Time Planner](https://minwoo19930301.github.io/tour-time-planner/)
- GitHub: [minwoo19930301/tour-time-planner](https://github.com/minwoo19930301/tour-time-planner)

## 주요 기능

- 시간 x 일차 테이블로 여행 일정 작성
- 여행 시작일 기준 날짜 자동 생성
- 셀 단건 편집과 다중 선택 일괄 편집
- 일정 제목, 배경색, 이동 수단 아이콘, 메모, 지도 링크 입력
- 드래그 앤 드롭으로 일정 카드 이동
- 공유 링크 생성 및 공유 링크 불러오기
- `localStorage` 자동 저장
- 모바일 터치 환경에서 드래그 편집 지원

## 사용하는 방법

1. 앱을 열고 새 일정 생성 또는 공유 링크 열기를 선택합니다.
2. 여행 시작일을 지정하면 `1일차`, `2일차` 형식으로 날짜가 자동으로 채워집니다.
3. `⊕ 일차 추가`, `⊖ 일차 제거`로 일정 길이를 조정합니다.
4. 시간표 셀을 눌러 일정을 입력합니다. 여러 칸을 선택하면 한 번에 수정할 수 있습니다.
5. 일정 이름, 색상, 아이콘, 메모, 지도 링크를 저장합니다.
6. 필요하면 일정 카드를 다른 시간대로 드래그해서 옮깁니다.
7. 공유 기능으로 생성한 링크를 복사해 다른 사람에게 전달합니다.

## 로컬 실행

정적 파일만으로 구성되어 있어 간단한 HTTP 서버로 바로 실행할 수 있습니다.

```bash
python3 -m http.server 4173 --bind 127.0.0.1 --directory "/Users/minwokim/Documents/New project/tour-schedular"
```

브라우저에서 `http://127.0.0.1:4173`를 열면 됩니다.

## 배포

- GitHub Pages: [https://minwoo19930301.github.io/tour-time-planner/](https://minwoo19930301.github.io/tour-time-planner/)
- 별도 빌드 과정 없이 정적 파일 배포

## 구현 메모 및 서브 상세 설명서

- 단일 `index.html`에 UI와 로직이 함께 들어 있습니다.
- `Tailwind CSS CDN`을 사용합니다.
- 모바일 드래그 처리를 위해 `DragDropTouch`를 사용합니다.
- 📘 **[시스템 아키텍처 및 상세 개발자 매뉴얼](docs/MANUAL.md)**: 매트릭스 스케줄러 아키텍처, 터치 드래그 연동 및 데이터 공유 프로토콜

## 📄 라이선스 (License)

본 프로젝트는 **[CC BY-NC 4.0 (크리에이티브 커먼즈 저작자표시-비영리 4.0)](LICENSE)** 라이선스에 따라 개인 및 비영리 목적으로 자유롭게 사용하실 수 있습니다.

> ⚠️ **상업적 이용 안내**: 기업 사용, 유료 서비스 연동, 외주 개발 등 상업적 목적으로 활용 시 저작권자(`contact@ai-ing.org`)와 **별도의 상업 라이선스 계약**을 체결해야 합니다.