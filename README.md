# Dev::Portfolio

> 학습 과정과 프로젝트 진행 중 마주친 문제들, 해결 과정을 기록하는 개인 포트폴리오 웹사이트

## Overview

단순한 이력서형 포트폴리오가 아닌, **왜 이렇게 설계했는가** · **어떤 문제를 만났는가** · **어떻게 해결했는가**를 중심으로 작성된 기술 기록 공간입니다.
각 프로젝트와 학습 항목은 결과물뿐만 아니라 진행 과정에서의 의사결정, 트러블슈팅, 회고를 포함합니다.


## Contents

### Projects

| 프로젝트 | 설명 |
|---|---|
| `ml-based-attack-defense-system-in-sdn` | SDN 환경에서 ML을 활용한 네트워크 공격 탐지 및 자동 방어 시스템 |
| `vcis-crypto-investment-simulation` | 암호화폐 투자 시뮬레이션 시스템 |
| `toy-project` | 기술 실험 및 사이드 프로젝트 모음 |
| `this-web` | 현재 포트폴리오 웹사이트 (본 프로젝트) |

### Studies

| 학습 | 설명                       |
|---|--------------------------|
| `java-jungsuk-remind` | Jav의 정석 핵심 개념 복습 및 심화 정리 |
| `algorithm-study` | 알고리즘 문제풀이 및 패턴 분석        |

<br>

## Tech Stack

### Frontend
![React](https://img.shields.io/badge/React-20232A?style=flat&logo=react&logoColor=61DAFB)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)
![Axios](https://img.shields.io/badge/Axios-5A29E4?style=flat&logo=axios&logoColor=white)

### Backend
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat&logo=springboot&logoColor=white)
![Java](https://img.shields.io/badge/Java_21-ED8B00?style=flat&logo=openjdk&logoColor=white)
![Gradle](https://img.shields.io/badge/Gradle-02303A?style=flat&logo=gradle&logoColor=white)

### Database
![H2](https://img.shields.io/badge/H2-004088?style=flat&logo=h2&logoColor=white)

<br>

## Architecture

```
Frontend (React.js)
    │
    ├── GET  /api/projects?type=project   → 프로젝트 목록
    ├── GET  /api/projects?type=study     → 학습 목록
    ├── GET  /api/contents?keyword={q}   → 키워드 검색
    └── POST /api/contact                → 문의 메일 전송
    │
Backend (Spring Boot)
    │
    └── H2 Database (콘텐츠 및 메타데이터)
```

### API 흐름

- **Front → Back** : 키워드 기반 콘텐츠 검색 요청
- **Back → Front** : 본문 내용 및 페이지 콘텐츠 JSON 응답


## Project Structure

```
portfolio/
├── frontend/                   # React.js
│
├── backend/                    # Spring Boot
│
└── README.md
```

## Writing Focus

각 콘텐츠는 아래 관점을 중심으로 작성됩니다.

- **설계 의도** — 왜 이 방식을 선택했는가
- **문제와 해결** — 진행 중 마주친 이슈와 해결 과정
- **학습 포인트** — 이 과정에서 새롭게 알게 된 것

<br>

## Author

**jynoh00** · [GitHub](https://github.com/jynoh00)