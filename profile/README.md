# 연구실 GPU 서버 자원 예약 및 실시간 모니터링 시스템

[프로젝트 소개 사이트](https://2026-2-web-programming-term-project.github.io/) · [상세 WBS 초안](https://github.com/2026-2-web-programming-term-project/2026-2-web-programming-term-project.github.io/blob/main/docs/WBS.md)

연구실이 보유한 GPU 서버·노드의 상태를 확인하고 사용 시간을 예약하는 웹 서비스입니다. 연구원은 자원 상태·예약·알림·본인 이력을 확인하고, 관리자는 소속 연구실의 자원·회원·예약 정책과 통계를 관리합니다.

**2026학년도 2학기 웹 프로그래밍 텀프로젝트**

## 주요 기능

- 연구실 초대 코드 가입, 이메일 인증, 일반 사용자·관리자 권한 분리
- GPU 자원 모니터링, 갱신 시각과 연결 이상 표시
- 캘린더 예약, 수정·취소·조기 종료, 중복 예약과 연속 점유 제한
- 예약 임박·조기 종료 알림, 사용 이력과 예약 통계
- 관리자 운영 화면과 모바일 반응형 UI

예약 정보와 실제 GPU 사용 상태를 구분하며, 예약 처리가 GPU 작업의 자동 실행·강제 중지를 뜻하지 않습니다.

## 저장소

| 저장소 | 역할 |
| --- | --- |
| [Front](https://github.com/2026-2-web-programming-term-project/WP-TP-Front) | Thymeleaf, HTML·CSS·JavaScript 화면 |
| [Gateway](https://github.com/2026-2-web-programming-term-project/WP-TP-Gateway) | 서비스 라우팅과 공통 요청 처리 |
| [API](https://github.com/2026-2-web-programming-term-project/WP-TP-API) | 인증·자원·예약·알림·관리·통계 |
| [DB](https://github.com/2026-2-web-programming-term-project/WP-TP-DB) | 데이터 모델·스키마·DB 운영 |
| [Eureka](https://github.com/2026-2-web-programming-term-project/WP-TP-Eureka) | 서비스 등록과 디스커버리 |

## 제출 일정

| 단계 | 마감 · KST |
| --- | --- |
| 프론트엔드 | 2026-11-06 23:59 |
| JavaScript | 2026-11-20 23:59 |
| 백엔드 | 2026-12-04 23:59 |

## 인프라 방향

AWS Infrastructure Composer와 CloudFormation으로 인프라를 코드화하고, 다중 가용 영역·EC2 Auto Scaling을 이용한 HA와 수평 확장을 설계합니다. ALB·ACM 기반 HTTPS 진입점, 데이터 계층과 서비스 디스커버리의 장애 대응, 부하·복구 검증을 함께 다룰 계획입니다.

현재는 초기 프로젝트 구성 단계입니다. 서비스 기능과 인프라는 구현·검증 예정이며, 운영 배포나 트래픽 처리 성능을 검증한 상태는 아닙니다.

[프로젝트 상세 소개와 인프라 설계 방향](https://github.com/2026-2-web-programming-term-project/.github/blob/main/README.md)
