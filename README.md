# 🛣️ Highway Gourmet Road
> **전국 휴게소 맛집 및 여정 정보 큐레이션 시스템**
> 
> 고속도로 여행 중 최적의 휴게소와 맛집 메뉴를 쉽고 빠르게 추천받는 Flask 기반 웹 서비스입니다.

---

## 📌 프로젝트 개요
* **진행 기간:** 2025.12.09 ~ 2025.12.22
* **목표:** 단순 경로 안내를 넘어, AI 기반 메뉴 추천과 위치 정보를 결합하여 사용자에게 최적화된 휴게소 경험을 제공합니다.
* **주요 타겟:** 국내 자동차 여행객 및 고속도로 이용자

## 🛠 기술 스택
### Backend
- ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
- ![Flask](https://img.shields.io/badge/flask-%23000.svg?style=for-the-badge&logo=flask&logoColor=white)
- ![MariaDB](https://img.shields.io/badge/MariaDB-003545?style=for-the-badge&logo=mariadb&logoColor=white)

### Frontend
- ![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white)
- ![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E)
- ![TailwindCSS](https://img.shields.io/badge/tailwindcss-%2338B2AC.svg?style=for-the-badge&logo=tailwind-css&logoColor=white)

### API & Tools
- **Google Gemini API**: AI 기반 메뉴 추천 및 큐레이션
- **Kakao Maps API**: 실시간 경로 탐색 및 마커 시각화

## ✨ 주요 기능
### 1. 실시간 경로 및 휴게소 필터링
- 출발지와 목적지 입력 시 최적 경로 산출
- 경로 반경 1.5km 이내의 휴게소 자동 검색
- 상/하행 방향 판별을 통한 정확한 정보 제공

### 2. AI 메뉴 추천 (Gemini 연동)
- 각 휴게소의 대표 메뉴 데이터를 Gemini API로 분석
- 사용자에게 유익한 메뉴 상세 설명 및 특징 요약 제공

### 3. 편의시설 정보 및 위치 연동
- 주유소, 전기차 충전소, 약국, 수유실 등 필수 시설 정보 표출
- 카카오맵 위치보기 링크 연동으로 즉시 내비게이션 연결 가능

## 🏗 시스템 구조 (Architecture)


1. **Client**: 사용자 입력 및 Kakao Maps 시각화 (JavaScript, main.js)
2. **Server**: 비즈니스 로직 처리 및 API 통신 (Python, app.py)
3. **Database**: 전국 휴게소 및 메뉴 데이터 관리 (MariaDB, db.py)
4. **AI Layer**: 메뉴 큐레이션 생성 (Google Gemini)

## 👥 팀원 및 역할
| 이름 | 역할 | 담당 영역 |
| :--- | :---: | :--- |
| **박민우** | PM | 프로젝트 총괄, 일정 관리 및 리소스 배분 |
| **신민서** | PL | 시스템 아키텍처 설계, 백엔드 핵심 로직 개발 |
| **이유진** | UI/UX | 프론트엔드 디자인 및 화면 구현, 사용자 경험 최적화 |
| **류건우** | AI/API | Gemini API 연동 및 AI 추천 로직 구현 |
| **권민지** | DB/Deploy | MariaDB 스키마 설계 및 서버 배포 환경 구축 |

## 🚀 향후 계획
- 카카오맵 기반 실시간 도로 혼잡도 연동
- 사용자 선호도 기반 맞춤형 음식 카테고리 추천
- 카카오내비 앱 직접 연동 기능 추가
