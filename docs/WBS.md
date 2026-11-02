# GitHub Projects WBS

실제 작업 일정과 진행 상태는 **[오거니제이션의 통합 WBS Projects](https://github.com/orgs/2026-2-web-programming-term-project/projects/1)**에서 관리합니다. 이 파일은 Projects로 연결하는 안내입니다.

## 보기

| 보기 | 용도 |
| --- | --- |
| [통합 WBS](https://github.com/orgs/2026-2-web-programming-term-project/projects/1/views/1) | 59개 작업의 저장소·단계·상태·일정·선행·완료 기준 |
| [저장소별 WBS](https://github.com/orgs/2026-2-web-programming-term-project/projects/1/views/4) | 담당 저장소로 묶은 작업 목록 |
| [진행 상태](https://github.com/orgs/2026-2-web-programming-term-project/projects/1/views/5) | 예정·진행·검증 중·완료 상태 보드 |
| [일정](https://github.com/orgs/2026-2-web-programming-term-project/projects/1/views/6) | 시작일·목표일을 사용하는 로드맵 |

## 필드와 관리 기준

- `WBS ID`: FE·JS·FR·API·GW·DB·EU·INF·INT·DOC 작업 식별자
- `저장소`·`단계`: 담당 영역과 제출 단계별 구분
- `Start date`·`Target date`: 계획 시작일과 목표 완료일
- `제출 마감`: 일 단위 마감. 제출 시각은 아래의 한국 시간 23:59 적용
- `선행 작업`·`완료 기준`: 착수 조건과 완료 판정에 필요한 내용
- `Status`: 예정 → 진행 → 검증 중 → 완료

각 항목의 상세 설명에도 담당 저장소·일정·선행·완료 기준을 기록했습니다. 작업 카드의 완료 기준을 검증한 뒤 상태를 변경합니다. 날짜가 지났다는 이유로 완료 처리하지 않습니다.

## 제출 마감

| 단계 | 마감 · KST |
| --- | --- |
| 프론트엔드 | 2026-11-06 23:59 |
| JavaScript | 2026-11-20 23:59 |
| 백엔드 | 2026-12-04 23:59 |

소개 사이트·문서 작업과 실제 서비스 Front 구현 진척은 구분합니다. 인프라 작업은 별도 단계로 추적하며 IaC 코드 보관 위치는 INF-01에서 확정합니다.

이전 Markdown 계획표는 [기준선 이력](https://github.com/2026-2-web-programming-term-project/.github/blob/8bcf27d186227f3da786117ed3e2a991dff8550b/docs/WBS.md)으로 남아 있습니다. 현재 일정·상태는 Projects를 기준으로 확인합니다.
