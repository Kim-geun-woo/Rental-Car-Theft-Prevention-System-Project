# 공유렌트카 도용 방지 시스템

**Python 기반 얼굴 인식 및 챗봇 연동을 통한 신분증 도용 방지 시스템**

---

## 📌 프로젝트 개요

공유 렌트카에서 발생하는 **신분증 도용** 및 **무면허 운전** 등의 범죄를 방지하기 위해  
**OpenCV와 얼굴 인식 API, Telegram Bot API**를 활용한 실시간 인증 시스템을 구현했습니다.

- **수행 기간**: 2023년 1학기  
- **수행 과목**: 멀티미디어 신호처리  
- **팀원 수**: 4명  
- **프로젝트 유형**: 팀 프로젝트 (설계 + 구현 + 발표)

---

## 👤 팀원 및 역할

| 이름       | 역할 1                  | 역할 2                    |
|------------|--------------------------|----------------------------|
| 팀원 A     | 기술 구현                | 검토                       |
| **(본인)** | 얼굴 인식 기능 구현 보조 | 검토                       |
| 팀원 B     | 아이디어 제안            | 리플렛 제출                |
| 팀원 C     | PPT 제작                 | 최종 발표                  |

---

## 🛠️ 주요 기능

- 차량 내 카메라로 운전자의 얼굴을 촬영
- 미리 등록된 **신분증 사진**과 대조하여 동일 인물 여부 확인
- **OpenCV + face_recognition API**로 실시간 얼굴 인식
- 불일치 시 **Telegram Bot API**를 통해 관리자에게 실시간 경고 메시지 전송
- 사용자 로그 및 상황 모니터링 기능 포함

---

## 📂 주요 산출물

- `camera.py` - 카메라 제어 및 실시간 촬영
- `face_classifier.py` - 얼굴 인식 분류기
- `face_recog.py` - 얼굴 비교 및 판별 로직
- `main.py` - 시스템 통합 실행 메인 파일
- `visitor_alarm_telegram_bot.py` - 관리자 알림 전송용 봇
- `templates/` - 웹 스트리밍 템플릿
- `knowns/`, `result/` - 입력 및 결과 저장 디렉토리 (`.gitkeep` 포함)

---

## 🎥 시연 영상

- 📽️ [Telegram 봇 시연 영상](https://youtube.com/shorts/Ox8f2rt5Z0U?feature=share)
- 📽️ [얼굴 인식 동작 영상](https://youtube.com/shorts/UaI0TedMhJQ?feature=share)

---

## 🧠 사용 기술

- Python  
- OpenCV  
- face_recognition  
- Telegram Bot API  
- Slack, Notion, GitHub

---

## 🔐 특허 가능성

- 기존 신분증 판별기는 단순 재질/형태 식별에 국한됨
- 본 시스템은 **실제 사용자와 신분증 사진의 일치 여부를 인식**,  
  범죄 예방에 직접적으로 기여하는 기능으로 **차별성 확보**

---

## 📎 관련 링크

- 발표 자료 PDF: [`docs/멀티미디어신호처리_TEAM_ARMY_TIGER_최종발표.pdf`](https://github.com/Kim-geun-woo/Rental-Car-Theft-Prevention-System-Project/blob/main/docs/%EB%A9%80%ED%8B%B0%EB%AF%B8%EB%94%94%EC%96%B4%EC%8B%A0%ED%98%B8%EC%B2%98%EB%A6%AC_TEAM_ARMY_TIGER_%EC%B5%9C%EC%A2%85%EB%B0%9C%ED%91%9C.pdf)
- Notion: [프로젝트 문서 정리 페이지](https://picturesque-lunch-045.notion.site/306b2b04d5ae40ae8d0092c35cc3ad56?v=8ba4b28f5f594e75a6016985db4b8941&pvs=74)

---

## ✅ 향후 확장 계획

- 외형 변화 (안경 착용 등)에 따른 인식률 보완
- 차량 내 **이상 행동 감지** 및 경고 기능 추가
- GPS와 연동된 이동 경로 추적 기능 개발
"""
