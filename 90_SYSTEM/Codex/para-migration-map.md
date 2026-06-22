# PARA Migration Map

작성일: 2026-06-22
업데이트: 2026-06-22, `AGENTS.md` Vault Rules 반영

## 전제

- 이 문서는 Tiago Forte의 PARA Method 기준으로 Vault 재구성 후보만 정리한 분류표이다.
- 이 단계에서는 파일을 이동하지 않았다.
- 원본 노트 내용은 수정하지 않았다.
- 새 내부링크를 삽입하지 않았다.
- `.git` 폴더는 분류 대상에서 제외했다.
- 조사 시점 기준 파일 수는 `.git` 제외 140개이다.
- 현재 워킹트리에는 이전 단계의 Markdown 형식 정리 변경이 남아 있다. 이 문서는 그 변경을 되돌리거나 추가 수정하지 않는다.
- 분류 판단은 주제명보다 현재성, 실행성, 완료 기준, 민감자료 여부를 우선한다.

## PARA 기준

| 코드 | 의미 | 기준 |
| --- | --- | --- |
| `00_INBOX` | 임시 수집함 | 정리되지 않은 임시 자료, 빈 노트, 성격이 불분명한 입력물 |
| `10_PROJECTS` | 프로젝트 | 현재 진행 중이고 완료 기준, 전시, 제출, 마감, 결과물이 있는 작업 |
| `20_AREAS` | 영역 | 장기적으로 유지해야 하는 책임 영역, 반복 운영, 관계/협업 단위 |
| `30_RESOURCES` | 자료 | 미래에 참고할 주제, 작가, 이론, 제작 방식, 기술 자료 |
| `40_ARCHIVES` | 보관 | 완료되었거나 비활성화된 자료, 과거 이벤트 기록 |
| `50_MAPS` | 지도 | MOC, 인덱스, Bases, 컬렉션 뷰 |
| `90_SYSTEM` | 시스템 | Obsidian 설정, 첨부파일, Codex 보고서, 스크립트, 운영 파일 |

## 적용한 Vault Rules

- 프로젝트는 완료 기준, 마감, 전시, 제출, 산출물이 확인될 때만 `10_PROJECTS`로 둔다.
- 장기 협업, 교육 프로그램, 반복 운영은 완료되지 않는 책임 영역으로 보고 `20_AREAS` 후보로 둔다.
- 작가, 장비, 제작 방식, 이론, 시각 모티프는 현재 프로젝트에 쓰였더라도 독립 참고성이 강하면 `30_RESOURCES` 후보로 둔다.
- 과거 발표, 참여하지 않을 예정인 행사, 비활성 기록은 `40_ARCHIVES` 후보로 둔다.
- 빈 노트, 제목 없는 노트, 성격이 불명확한 Bases 파일은 이동 제안 없이 `review-needed`로 둔다.
- 학생 개인정보, 평가자료, 민감 자료 가능성이 있는 파일은 `review-needed-sensitive`로 표시하고 이동 전 사용자 확인을 요구한다.
- 폴더 이동은 의미 연결을 대체하지 않으므로, MOC/내부링크 설계는 별도 작업으로 둔다.
- `AGENTS.md`는 Vault 운영 규칙이므로 루트에 유지한다.

## 폴더 분류표

| 현재 폴더 | 추정 성격 | 제안 위치 | confidence | 상태 |
| --- | --- | --- | --- | --- |
| `.` | Vault 루트 | PARA 루트 구조로 재편: `00_INBOX`, `10_PROJECTS`, `20_AREAS`, `30_RESOURCES`, `40_ARCHIVES`, `50_MAPS`, `90_SYSTEM` | high | 제안 |
| `.obsidian` | Obsidian 앱 설정 | 이동 없음: `.obsidian` 유지 | high | system-fixed |
| `.obsidian/plugins` | Obsidian 플러그인 | 이동 없음: `.obsidian/plugins` 유지 | high | system-fixed |
| `.obsidian/plugins/calendar` | Calendar 플러그인 | 이동 없음 | high | system-fixed |
| `.obsidian/plugins/templater-obsidian` | Templater 플러그인 | 이동 없음 | high | system-fixed |
| `.obsidian/themes` | Obsidian 테마 | 이동 없음 | high | system-fixed |
| `00_SYSTEM` | Codex/시스템 보고서 | `90_SYSTEM/Codex` | high | 제안 |
| `00_SYSTEM/Troubleshooting` | 운영 문제 해결 기록 | `90_SYSTEM/Codex/Troubleshooting` | high | 제안 |
| `Arkive` | 과거/임시 보관 | 주로 `40_ARCHIVES`, 일부 `30_RESOURCES` 또는 `00_INBOX` | medium | split-needed |
| `Arkive/호반` | 교육 프로그램 관련 기록, 참여자/교육 맥락 포함 가능 | `20_AREAS/교육 프로그램` 또는 `40_ARCHIVES/교육 프로그램` | medium | review-needed-sensitive |
| `Work` | 작업 문서 혼합 폴더 | 프로젝트/영역/자료로 분할 | medium | split-needed |
| `Work/Research` | 논문 관련 진행 작업 | `10_PROJECTS/논문 26년도` | high | 제안 |
| `Work/Residence` | 레지던시/지원 프로젝트 | `10_PROJECTS/한불수교 140주년 Le Wonder` | high | 제안 |
| `Work/Transmitter to Object` | 진행 중 작업 프로젝트 | `10_PROJECTS/Transmitter to Object` | high | 제안 |
| `Work/Transmitter to Object/Shot_Plan` | 촬영 계획 | `10_PROJECTS/Transmitter to Object/Shot_Plan` | high | 제안 |
| `Work/Transmitter to Object/Tech` | 프로젝트 기술 메모 | `10_PROJECTS/Transmitter to Object/Tech` | high | 제안 |
| `Work/Transmitter to Object/Text_Plan` | 프로젝트 텍스트/설치 계획 | `10_PROJECTS/Transmitter to Object/Text_Plan` | high | 제안 |
| `Work/민족자결주의자를 위한 AI기술 활용` | 자결의 프로토콜 프로젝트 | `10_PROJECTS/자결의 프로토콜` | high | 제안 |
| `전시관련` | 전시/기관 접촉 문서 | 각 전시별 `10_PROJECTS` 또는 완료 문서는 `40_ARCHIVES` | medium | split-needed |
| `첨부파일` | Obsidian 첨부파일 | `90_SYSTEM/Attachments` | high | 제안 |
| `프로토콜 콜렉티브` | 장기 협업/운영 영역 | `20_AREAS/프로토콜 콜렉티브` | high | 제안 |
| `90_SYSTEM` | 새 시스템 루트 | `90_SYSTEM` 유지 | high | 생성됨 |
| `90_SYSTEM/Codex` | Codex 보고서/분류표 | `90_SYSTEM/Codex` 유지 | high | 생성됨 |

## Markdown 파일 분류표

| 현재 경로 | 추정 성격 | 제안 이동 경로 | confidence | 상태 |
| --- | --- | --- | --- | --- |
| `AGENTS.md` | Vault 운영 규칙 | 이동 없음: `AGENTS.md` | high | system-fixed |
| `00_SYSTEM/Troubleshooting/트러블 슈팅.md` | Codex/운영 트러블슈팅 | `90_SYSTEM/Codex/Troubleshooting/트러블 슈팅.md` | high | 제안 |
| `00_SYSTEM/link-suggestions.md` | Codex 내부링크 제안 보고서 | `90_SYSTEM/Codex/link-suggestions.md` | high | 제안 |
| `00_SYSTEM/semantic-link-suggestions.md` | Codex 의미 링크 제안 보고서 | `90_SYSTEM/Codex/semantic-link-suggestions.md` | high | 제안 |
| `Arkive/10.29  질문들.md` | 과거 질문/이벤트 기록 | `40_ARCHIVES/Events/10.29  질문들.md` | medium | 제안 |
| `Arkive/25.12.27작업 키워드 정1리.md` | 빈 노트/임시 입력물 | `00_INBOX/25.12.27작업 키워드 정1리.md` | medium | 제안 |
| `Arkive/26.01.10 한미 프리젠테이션.md` | 한미사진미술관/전시 준비와 연결될 수 있는 발표 기록 | `10_PROJECTS/한미사진미술관/Research/26.01.10 한미 프리젠테이션.md` | medium | 제안 |
| `Arkive/26.02.28 무진형제.md` | 작가/토크 참고 자료 | `30_RESOURCES/Artists/무진형제/26.02.28 무진형제.md` | medium | 제안 |
| `Arkive/26.04 서사축.md` | 짧은 임시 메모 | `review-needed` | low | review-needed |
| `Arkive/3D 프린터.md` | 제작 장비 참고 자료 | `30_RESOURCES/제작기술/3D 프린터.md` | high | 제안 |
| `Arkive/사월의 눈 25.05.07.md` | 작업 레퍼런스/시각 모티프 | `30_RESOURCES/작업 레퍼런스/사월의 눈 25.05.07.md` | medium | 제안 |
| `Arkive/호반/교육프로그램.md` | 교육 프로그램 운영/기획, 참여자/교육 맥락 포함 가능 | `20_AREAS/교육 프로그램/호반 교육프로그램.md` | medium | review-needed-sensitive |
| `Work/Research/논문 26년도.md` | 2026 논문 프로젝트 | `10_PROJECTS/논문 26년도/논문 26년도.md` | high | 제안 |
| `Work/Residence/26년도  한불수교 140주년 Le. wonder.md` | 레지던시/지원 프로젝트 | `10_PROJECTS/한불수교 140주년 Le Wonder/26년도 한불수교 140주년 Le. wonder.md` | high | 제안 |
| `Work/Transmitter to Object/25.12.27작업 키워드 정리-인쇄필요.md` | Transmitter to Object 키워드/기획 | `10_PROJECTS/Transmitter to Object/Planning/25.12.27작업 키워드 정리-인쇄필요.md` | high | 제안 |
| `Work/Transmitter to Object/Keyword_랜스미터 투 더 오브젝트 - 오리엔티드 데이터.md` | Transmitter to Object 개념/데이터 기획 | `10_PROJECTS/Transmitter to Object/Planning/Keyword_랜스미터 투 더 오브젝트 - 오리엔티드 데이터.md` | high | 제안 |
| `Work/Transmitter to Object/Shot_Plan/25년도 촬영 계획.md` | Transmitter to Object 촬영 계획 | `10_PROJECTS/Transmitter to Object/Shot_Plan/25년도 촬영 계획.md` | high | 제안 |
| `Work/Transmitter to Object/Shot_Plan/26년도 촬영 계획.md` | Transmitter to Object 촬영 계획 | `10_PROJECTS/Transmitter to Object/Shot_Plan/26년도 촬영 계획.md` | high | 제안 |
| `Work/Transmitter to Object/Shot_Plan/Video_영상작업.md` | Transmitter to Object 영상 계획 | `10_PROJECTS/Transmitter to Object/Shot_Plan/Video_영상작업.md` | high | 제안 |
| `Work/Transmitter to Object/Shot_Plan/라이카 Sofort 카메라.md` | Transmitter to Object 촬영/카메라 레퍼런스 | `10_PROJECTS/Transmitter to Object/Shot_Plan/라이카 Sofort 카메라.md` | medium | 제안 |
| `Work/Transmitter to Object/Shot_Plan/동체시력.md` | Transmitter to Object 촬영 개념/시각 자료 | `10_PROJECTS/Transmitter to Object/Shot_Plan/동체시력.md` | medium | 제안 |
| `Work/Transmitter to Object/Tech/05.14 SVG.md` | Transmitter to Object 기술 메모 | `10_PROJECTS/Transmitter to Object/Tech/05.14 SVG.md` | high | 제안 |
| `Work/Transmitter to Object/Tech/chat gpt라인-포인트 from csv.md` | Transmitter to Object 데이터 처리 프롬프트/절차 | `10_PROJECTS/Transmitter to Object/Tech/chat gpt라인-포인트 from csv.md` | high | 제안 |
| `Work/Transmitter to Object/Text_Plan/26년 전시 - Reference.md` | Transmitter to Object 전시 레퍼런스 | `10_PROJECTS/Transmitter to Object/Text_Plan/26년 전시 - Reference.md` | high | 제안 |
| `Work/Transmitter to Object/Text_Plan/Artist Statement 아티스트 스테이트먼트.md` | Transmitter to Object 작가노트 | `10_PROJECTS/Transmitter to Object/Text_Plan/Artist Statement 아티스트 스테이트먼트.md` | high | 제안 |
| `Work/Transmitter to Object/Text_Plan/PLACE 장소 & intallation 설치.md` | Transmitter to Object 장소/설치 계획 | `10_PROJECTS/Transmitter to Object/Text_Plan/PLACE 장소 & intallation 설치.md` | high | 제안 |
| `Work/민족자결주의자를 위한 AI기술 활용/<자결의 프로토콜> 계획서 05.21.md` | 자결의 프로토콜 구현 계획 | `10_PROJECTS/자결의 프로토콜/Planning/<자결의 프로토콜> 계획서 05.21.md` | high | 제안 |
| `Work/민족자결주의자를 위한 AI기술 활용/계획서.md` | 자결의 프로토콜 임시 계획 | `10_PROJECTS/자결의 프로토콜/Planning/계획서.md` | medium | 제안 |
| `Work/민족자결주의자를 위한 AI기술 활용/민족자결주의자를 위한 기술선언.md` | 자결의 프로토콜 리서치/선언문 자료 | `10_PROJECTS/자결의 프로토콜/Research/민족자결주의자를 위한 기술선언.md` | high | 제안 |
| `Work/민족자결주의자를 위한 AI기술 활용/무제.md` | 제목 없는 프로젝트 메모 | `review-needed` | low | review-needed |
| `Work/민족자결주의자를 위한 AI기술 활용/자결의 프로토콜 Protocol of Self-Determination.md` | 자결의 프로토콜 텍스트/구성안 | `10_PROJECTS/자결의 프로토콜/Texts/자결의 프로토콜 Protocol of Self-Determination.md` | high | 제안 |
| `Work/탈식민주의 시대의 예술이 다루는 주제.md` | 이론/주제 참고 자료 | `30_RESOURCES/이론_주제/탈식민주의 시대의 예술이 다루는 주제.md` | high | 제안 |
| `Work/프린팅 방식.md` | 제작 방식 참고 자료 | `30_RESOURCES/제작기술/프린팅 방식.md` | high | 제안 |
| `cleanup-plan.md` | Codex cleanup 계획 보고서 | `90_SYSTEM/Codex/cleanup-plan.md` | high | 제안 |
| `cleanup-report.md` | Codex cleanup 분석 보고서 | `90_SYSTEM/Codex/cleanup-report.md` | high | 제안 |
| `전시관련/[26년] 접촉화면.md` | 접촉화면 전시 프로젝트 | `10_PROJECTS/접촉화면/[26년] 접촉화면.md` | high | 제안 |
| `전시관련/[26년] 광비 GB토크.md` | 비활성/참여 예정 없음으로 보이는 토크 기록 | `40_ARCHIVES/전시관련/[26년] 광비 GB토크.md` | medium | 제안 |
| `전시관련/[27년] 한미사진미술관.md` | 한미사진미술관 전시 프로젝트 | `10_PROJECTS/한미사진미술관/[27년] 한미사진미술관.md` | high | 제안 |
| `프로토콜 콜렉티브/25.01.19.md` | 장기 협업 영역의 날짜 기록 | `20_AREAS/프로토콜 콜렉티브/25.01.19.md` | high | 제안 |
| `프로토콜 콜렉티브/25.01.22.md` | 장기 협업 영역의 날짜 기록 | `20_AREAS/프로토콜 콜렉티브/25.01.22.md` | high | 제안 |
| `90_SYSTEM/Codex/para-migration-map.md` | Codex PARA 분류표 | `90_SYSTEM/Codex/para-migration-map.md` | high | 유지 |

## 최근 수정 파일 기준 재분류 요약

최근 수정 여부는 Markdown 형식 정리 작업의 결과일 수 있으므로, 그 자체를 프로젝트 판단 근거로 삼지 않는다. 아래 판단은 최근 수정 파일의 내부 내용과 현재성/실행성 기준을 함께 본 것이다.

| 묶음 | 해당 파일 예시 | 분류 판단 | 이유 |
| --- | --- | --- | --- |
| 현재 전시/작업 산출물 | `Work/Transmitter to Object/*`, `전시관련/[26년] 접촉화면.md`, `전시관련/[27년] 한미사진미술관.md` | `10_PROJECTS` | 촬영, 설치, 텍스트, 전시 구성처럼 결과물과 실행 단위가 있음 |
| 자결의 프로토콜 | `Work/민족자결주의자를 위한 AI기술 활용/*` | `10_PROJECTS` | 계획서, 구현 방향, 선언문/이미지 시스템이 산출물 단위로 연결됨 |
| 제출/지원/연구 | `Work/Research/논문 26년도.md`, `Work/Residence/26년도  한불수교 140주년 Le. wonder.md` | `10_PROJECTS` | 논문, 레지던시/지원처럼 완료 기준과 마감 가능성이 있음 |
| 장기 협업 | `프로토콜 콜렉티브/25.01.19.md`, `프로토콜 콜렉티브/25.01.22.md` | `20_AREAS` | 날짜 기록이지만 협업 단위가 지속 관리되는 영역임 |
| 참고 자료 | `Arkive/3D 프린터.md`, `Work/프린팅 방식.md`, `Work/탈식민주의 시대의 예술이 다루는 주제.md` | `30_RESOURCES` | 현재 프로젝트에 쓰일 수 있으나 특정 마감보다 참고성이 강함 |
| 과거/비활성 기록 | `전시관련/[26년] 광비 GB토크.md`, 일부 `Arkive/*` | `40_ARCHIVES` | 참여하지 않을 예정이거나 과거 이벤트 기록으로 보임 |
| 민감/확인 필요 | `Arkive/호반/교육프로그램.md`, `무제*.base`, `Work/민족자결주의자를 위한 AI기술 활용/무제.md` | `review-needed` / `review-needed-sensitive` | 교육/참여자 맥락, 제목 없음, 역할 불명확성 때문에 이동 전 확인 필요 |

## Obsidian 설정/플러그인 파일 분류표

주의: `.obsidian` 아래 파일은 Obsidian 앱이 직접 참조하므로 실제 이동 대상으로 보지 않는다. PARA상 시스템 파일로 분류하되 현재 위치 유지를 제안한다.

| 현재 경로 | 추정 성격 | 제안 이동 경로 | confidence | 상태 |
| --- | --- | --- | --- | --- |
| `.obsidian/.DS_Store` | macOS 시스템 부산물 | `review-needed` | low | review-needed |
| `.obsidian/app.json` | Obsidian 설정 | 이동 없음: `.obsidian/app.json` | high | system-fixed |
| `.obsidian/appearance.json` | Obsidian 외관 설정 | 이동 없음: `.obsidian/appearance.json` | high | system-fixed |
| `.obsidian/backlink.json` | Obsidian 백링크 설정 | 이동 없음: `.obsidian/backlink.json` | high | system-fixed |
| `.obsidian/community-plugins.json` | 커뮤니티 플러그인 설정 | 이동 없음: `.obsidian/community-plugins.json` | high | system-fixed |
| `.obsidian/core-plugins-migration.json` | 코어 플러그인 마이그레이션 설정 | 이동 없음: `.obsidian/core-plugins-migration.json` | high | system-fixed |
| `.obsidian/core-plugins.json` | 코어 플러그인 설정 | 이동 없음: `.obsidian/core-plugins.json` | high | system-fixed |
| `.obsidian/graph.json` | 그래프 설정 | 이동 없음: `.obsidian/graph.json` | high | system-fixed |
| `.obsidian/hotkeys.json` | 단축키 설정 | 이동 없음: `.obsidian/hotkeys.json` | high | system-fixed |
| `.obsidian/templates.json` | 템플릿 플러그인 설정 | 이동 없음: `.obsidian/templates.json` | high | system-fixed |
| `.obsidian/workspace-mobile.json` | 모바일 작업공간 상태 | 이동 없음: `.obsidian/workspace-mobile.json` | high | system-fixed |
| `.obsidian/workspace.json` | 데스크톱 작업공간 상태 | 이동 없음: `.obsidian/workspace.json` | high | system-fixed |
| `.obsidian/plugins/calendar/data.json` | Calendar 플러그인 데이터 | 이동 없음 | high | system-fixed |
| `.obsidian/plugins/calendar/main.js` | Calendar 플러그인 스크립트 | 이동 없음 | high | system-fixed |
| `.obsidian/plugins/calendar/manifest.json` | Calendar 플러그인 매니페스트 | 이동 없음 | high | system-fixed |
| `.obsidian/plugins/templater-obsidian/main.js` | Templater 플러그인 스크립트 | 이동 없음 | high | system-fixed |
| `.obsidian/plugins/templater-obsidian/manifest.json` | Templater 플러그인 매니페스트 | 이동 없음 | high | system-fixed |
| `.obsidian/plugins/templater-obsidian/styles.css` | Templater 플러그인 스타일 | 이동 없음 | high | system-fixed |
| `.obsidian/themes/Blue Topaz/manifest.json` | Obsidian 테마 매니페스트 | 이동 없음 | high | system-fixed |
| `.obsidian/themes/Blue Topaz/theme.css` | Obsidian 테마 스타일 | 이동 없음 | high | system-fixed |
| `.obsidian/themes/Minimal/manifest.json` | Obsidian 테마 매니페스트 | 이동 없음 | high | system-fixed |
| `.obsidian/themes/Minimal/theme.css` | Obsidian 테마 스타일 | 이동 없음 | high | system-fixed |
| `.obsidian/themes/Pink Topaz/manifest.json` | Obsidian 테마 매니페스트 | 이동 없음 | high | system-fixed |
| `.obsidian/themes/Pink Topaz/theme.css` | Obsidian 테마 스타일 | 이동 없음 | high | system-fixed |
| `.obsidian/themes/Sanctum/manifest.json` | Obsidian 테마 매니페스트 | 이동 없음 | high | system-fixed |
| `.obsidian/themes/Sanctum/theme.css` | Obsidian 테마 스타일 | 이동 없음 | high | system-fixed |
| `.obsidian/themes/Solarized/manifest.json` | Obsidian 테마 매니페스트 | 이동 없음 | high | system-fixed |
| `.obsidian/themes/Solarized/theme.css` | Obsidian 테마 스타일 | 이동 없음 | high | system-fixed |
| `.obsidian/themes/Things/manifest.json` | Obsidian 테마 매니페스트 | 이동 없음 | high | system-fixed |
| `.obsidian/themes/Things/theme.css` | Obsidian 테마 스타일 | 이동 없음 | high | system-fixed |
| `.obsidian/themes/Wasp/manifest.json` | Obsidian 테마 매니페스트 | 이동 없음 | high | system-fixed |
| `.obsidian/themes/Wasp/theme.css` | Obsidian 테마 스타일 | 이동 없음 | high | system-fixed |

## 시스템/루트 기타 파일 분류표

| 현재 경로 | 추정 성격 | 제안 이동 경로 | confidence | 상태 |
| --- | --- | --- | --- | --- |
| `.DS_Store` | macOS 시스템 부산물 | `review-needed` | low | review-needed |
| `.gitignore` | Git 운영 파일 | 이동 없음: `.gitignore` | high | system-fixed |
| `Work/.DS_Store` | macOS 시스템 부산물 | `review-needed` | low | review-needed |
| `무제.base` | Obsidian Bases 인덱스 후보, 제목 없음 | `review-needed` | low | review-needed |
| `무제 1.base` | Obsidian Bases 인덱스 후보, 제목 없음 | `review-needed` | low | review-needed |
| `무제 2.base` | Obsidian Bases 인덱스 후보, 제목 없음 | `review-needed` | low | review-needed |
| `무제 3.base` | Obsidian Bases 인덱스 후보, 제목 없음 | `review-needed` | low | review-needed |
| `무제 4.base` | Obsidian Bases 인덱스 후보, 제목 없음 | `review-needed` | low | review-needed |
| `무제 5.base` | Obsidian Bases 인덱스 후보, 제목 없음 | `review-needed` | low | review-needed |
| `무제 6.base` | Obsidian Bases 인덱스 후보, 제목 없음 | `review-needed` | low | review-needed |

## 첨부파일 분류표

| 현재 경로 | 추정 성격 | 제안 이동 경로 | confidence | 상태 |
| --- | --- | --- | --- | --- |
| `첨부파일/Golovin-Sivtsev_Table.svg.png` | Obsidian 첨부 이미지 | `90_SYSTEM/Attachments/Golovin-Sivtsev_Table.svg.png` | high | 제안 |
| `첨부파일/IMG_0431.png` | Obsidian 첨부 이미지 | `90_SYSTEM/Attachments/IMG_0431.png` | high | 제안 |
| `첨부파일/IMG_0443.png` | Obsidian 첨부 이미지 | `90_SYSTEM/Attachments/IMG_0443.png` | high | 제안 |
| `첨부파일/IMG_1590.jpeg` | Obsidian 첨부 이미지 | `90_SYSTEM/Attachments/IMG_1590.jpeg` | high | 제안 |
| `첨부파일/IMG_2373.jpeg` | Obsidian 첨부 이미지 | `90_SYSTEM/Attachments/IMG_2373.jpeg` | high | 제안 |
| `첨부파일/Image_fx (2).jpg` | Obsidian 첨부 이미지 | `90_SYSTEM/Attachments/Image_fx (2).jpg` | high | 제안 |
| `첨부파일/KakaoTalk_Photo_2025-05-30-17-28-18.jpeg` | Obsidian 첨부 이미지 | `90_SYSTEM/Attachments/KakaoTalk_Photo_2025-05-30-17-28-18.jpeg` | high | 제안 |
| `첨부파일/KakaoTalk_Photo_2026-03-23-00-52-14 002.jpeg` | Obsidian 첨부 이미지 | `90_SYSTEM/Attachments/KakaoTalk_Photo_2026-03-23-00-52-14 002.jpeg` | high | 제안 |
| `첨부파일/KakaoTalk_Photo_2026-03-23-00-52-14 003 1.jpeg` | Obsidian 첨부 이미지 | `90_SYSTEM/Attachments/KakaoTalk_Photo_2026-03-23-00-52-14 003 1.jpeg` | high | 제안 |
| `첨부파일/KakaoTalk_Photo_2026-03-23-00-52-14 003.jpeg` | Obsidian 첨부 이미지 | `90_SYSTEM/Attachments/KakaoTalk_Photo_2026-03-23-00-52-14 003.jpeg` | high | 제안 |
| `첨부파일/KakaoTalk_Photo_2026-03-23-00-52-14 005.jpeg` | Obsidian 첨부 이미지 | `90_SYSTEM/Attachments/KakaoTalk_Photo_2026-03-23-00-52-14 005.jpeg` | high | 제안 |
| `첨부파일/KakaoTalk_Photo_2026-03-23-00-52-14 006.jpeg` | Obsidian 첨부 이미지 | `90_SYSTEM/Attachments/KakaoTalk_Photo_2026-03-23-00-52-14 006.jpeg` | high | 제안 |
| `첨부파일/Landoltring_Abmessungen.jpg` | Obsidian 첨부 이미지 | `90_SYSTEM/Attachments/Landoltring_Abmessungen.jpg` | high | 제안 |
| `첨부파일/Screenshot 2025-04-14 at 21.13.53.png` | Obsidian 첨부 이미지 | `90_SYSTEM/Attachments/Screenshot 2025-04-14 at 21.13.53.png` | high | 제안 |
| `첨부파일/Screenshot 2025-04-23 at 10.49.57 PM.png` | Obsidian 첨부 이미지 | `90_SYSTEM/Attachments/Screenshot 2025-04-23 at 10.49.57 PM.png` | high | 제안 |
| `첨부파일/Screenshot 2025-04-23 at 11.05.39 PM.png` | Obsidian 첨부 이미지 | `90_SYSTEM/Attachments/Screenshot 2025-04-23 at 11.05.39 PM.png` | high | 제안 |
| `첨부파일/Screenshot 2025-04-23 at 11.32.34 PM.png` | Obsidian 첨부 이미지 | `90_SYSTEM/Attachments/Screenshot 2025-04-23 at 11.32.34 PM.png` | high | 제안 |
| `첨부파일/Screenshot 2025-04-23 at 11.35.33 PM.png` | Obsidian 첨부 이미지 | `90_SYSTEM/Attachments/Screenshot 2025-04-23 at 11.35.33 PM.png` | high | 제안 |
| `첨부파일/Screenshot 2025-04-23 at 11.37.48 PM.png` | Obsidian 첨부 이미지 | `90_SYSTEM/Attachments/Screenshot 2025-04-23 at 11.37.48 PM.png` | high | 제안 |
| `첨부파일/Screenshot 2025-05-08 at 00.49.02.png` | Obsidian 첨부 이미지 | `90_SYSTEM/Attachments/Screenshot 2025-05-08 at 00.49.02.png` | high | 제안 |
| `첨부파일/Screenshot 2025-05-14 at 18.16.04.png` | Obsidian 첨부 이미지 | `90_SYSTEM/Attachments/Screenshot 2025-05-14 at 18.16.04.png` | high | 제안 |
| `첨부파일/Screenshot 2025-06-08 at 23.50.42.png` | Obsidian 첨부 이미지 | `90_SYSTEM/Attachments/Screenshot 2025-06-08 at 23.50.42.png` | high | 제안 |
| `첨부파일/Screenshot 2025-08-01 at 11.56.11 PM.png` | Obsidian 첨부 이미지 | `90_SYSTEM/Attachments/Screenshot 2025-08-01 at 11.56.11 PM.png` | high | 제안 |
| `첨부파일/Screenshot 2025-08-02 at 12.06.26 AM 1.png` | Obsidian 첨부 이미지 | `90_SYSTEM/Attachments/Screenshot 2025-08-02 at 12.06.26 AM 1.png` | high | 제안 |
| `첨부파일/Screenshot 2025-08-02 at 12.06.26 AM.png` | Obsidian 첨부 이미지 | `90_SYSTEM/Attachments/Screenshot 2025-08-02 at 12.06.26 AM.png` | high | 제안 |
| `첨부파일/Screenshot 2025-08-07 at 14.00.56.png` | Obsidian 첨부 이미지 | `90_SYSTEM/Attachments/Screenshot 2025-08-07 at 14.00.56.png` | high | 제안 |
| `첨부파일/Screenshot 2025-08-26 at 17.57.12.png` | Obsidian 첨부 이미지 | `90_SYSTEM/Attachments/Screenshot 2025-08-26 at 17.57.12.png` | high | 제안 |
| `첨부파일/Screenshot 2025-08-31 at 23.16.20.png` | Obsidian 첨부 이미지 | `90_SYSTEM/Attachments/Screenshot 2025-08-31 at 23.16.20.png` | high | 제안 |
| `첨부파일/Screenshot 2025-10-17 at 14.28.24.png` | Obsidian 첨부 이미지 | `90_SYSTEM/Attachments/Screenshot 2025-10-17 at 14.28.24.png` | high | 제안 |
| `첨부파일/Screenshot 2025-11-01 at 2.44.26 PM.png` | Obsidian 첨부 이미지 | `90_SYSTEM/Attachments/Screenshot 2025-11-01 at 2.44.26 PM.png` | high | 제안 |
| `첨부파일/Screenshot 2025-11-01 at 2.44.47 PM 1.png` | Obsidian 첨부 이미지 | `90_SYSTEM/Attachments/Screenshot 2025-11-01 at 2.44.47 PM 1.png` | high | 제안 |
| `첨부파일/Screenshot 2025-11-01 at 2.44.47 PM.png` | Obsidian 첨부 이미지 | `90_SYSTEM/Attachments/Screenshot 2025-11-01 at 2.44.47 PM.png` | high | 제안 |
| `첨부파일/Screenshot 2025-11-24 at 22.01.50.png` | Obsidian 첨부 이미지 | `90_SYSTEM/Attachments/Screenshot 2025-11-24 at 22.01.50.png` | high | 제안 |
| `첨부파일/Screenshot 2026-03-16 at 23.36.18.png` | Obsidian 첨부 이미지 | `90_SYSTEM/Attachments/Screenshot 2026-03-16 at 23.36.18.png` | high | 제안 |
| `첨부파일/Screenshot 2026-03-24 at 11.53.07 PM.png` | Obsidian 첨부 이미지 | `90_SYSTEM/Attachments/Screenshot 2026-03-24 at 11.53.07 PM.png` | high | 제안 |
| `첨부파일/Screenshot 2026-03-24 at 23.31.14.png` | Obsidian 첨부 이미지 | `90_SYSTEM/Attachments/Screenshot 2026-03-24 at 23.31.14.png` | high | 제안 |
| `첨부파일/Screenshot 2026-03-24 at 23.31.50.png` | Obsidian 첨부 이미지 | `90_SYSTEM/Attachments/Screenshot 2026-03-24 at 23.31.50.png` | high | 제안 |
| `첨부파일/Screenshot 2026-03-24 at 23.39.20.png` | Obsidian 첨부 이미지 | `90_SYSTEM/Attachments/Screenshot 2026-03-24 at 23.39.20.png` | high | 제안 |
| `첨부파일/Screenshot 2026-03-25 at 12.07.02 AM 1.png` | Obsidian 첨부 이미지 | `90_SYSTEM/Attachments/Screenshot 2026-03-25 at 12.07.02 AM 1.png` | high | 제안 |
| `첨부파일/Screenshot 2026-03-25 at 12.07.02 AM 2.png` | Obsidian 첨부 이미지 | `90_SYSTEM/Attachments/Screenshot 2026-03-25 at 12.07.02 AM 2.png` | high | 제안 |
| `첨부파일/Screenshot 2026-03-25 at 12.07.02 AM 3.png` | Obsidian 첨부 이미지 | `90_SYSTEM/Attachments/Screenshot 2026-03-25 at 12.07.02 AM 3.png` | high | 제안 |
| `첨부파일/Screenshot 2026-03-25 at 12.07.02 AM.png` | Obsidian 첨부 이미지 | `90_SYSTEM/Attachments/Screenshot 2026-03-25 at 12.07.02 AM.png` | high | 제안 |
| `첨부파일/Screenshot 2026-03-26 at 10.13.20 AM.png` | Obsidian 첨부 이미지 | `90_SYSTEM/Attachments/Screenshot 2026-03-26 at 10.13.20 AM.png` | high | 제안 |
| `첨부파일/Screenshot 2026-04-13 at 16.33.25.png` | Obsidian 첨부 이미지 | `90_SYSTEM/Attachments/Screenshot 2026-04-13 at 16.33.25.png` | high | 제안 |
| `첨부파일/Screenshot 2026-04-20 at 15.56.47 1.png` | Obsidian 첨부 이미지 | `90_SYSTEM/Attachments/Screenshot 2026-04-20 at 15.56.47 1.png` | high | 제안 |
| `첨부파일/Screenshot 2026-04-20 at 15.56.47.png` | Obsidian 첨부 이미지 | `90_SYSTEM/Attachments/Screenshot 2026-04-20 at 15.56.47.png` | high | 제안 |
| `첨부파일/Screenshot 2026-04-20 at 15.57.40.png` | Obsidian 첨부 이미지 | `90_SYSTEM/Attachments/Screenshot 2026-04-20 at 15.57.40.png` | high | 제안 |
| `첨부파일/Screenshot 2026-05-26 at 18.14.54.png` | Obsidian 첨부 이미지 | `90_SYSTEM/Attachments/Screenshot 2026-05-26 at 18.14.54.png` | high | 제안 |
| `첨부파일/image7.jpg` | Obsidian 첨부 이미지 | `90_SYSTEM/Attachments/image7.jpg` | high | 제안 |
| `첨부파일/image_fx (1).jpg` | Obsidian 첨부 이미지 | `90_SYSTEM/Attachments/image_fx (1).jpg` | high | 제안 |
| `첨부파일/image_fx_ (7.jpg` | Obsidian 첨부 이미지 | `90_SYSTEM/Attachments/image_fx_ (7.jpg` | high | 제안 |
| `첨부파일/image_fx_ 1.jpg` | Obsidian 첨부 이미지 | `90_SYSTEM/Attachments/image_fx_ 1.jpg` | high | 제안 |
| `첨부파일/image_fx_ 2.jpg` | Obsidian 첨부 이미지 | `90_SYSTEM/Attachments/image_fx_ 2.jpg` | high | 제안 |
| `첨부파일/image_fx_.jpg` | Obsidian 첨부 이미지 | `90_SYSTEM/Attachments/image_fx_.jpg` | high | 제안 |
| `첨부파일/image_fx_1.jpg` | Obsidian 첨부 이미지 | `90_SYSTEM/Attachments/image_fx_1.jpg` | high | 제안 |
| `첨부파일/img11.6842ddc9.jpg` | Obsidian 첨부 이미지 | `90_SYSTEM/Attachments/img11.6842ddc9.jpg` | high | 제안 |
| `첨부파일/img16.b459881e.jpg` | Obsidian 첨부 이미지 | `90_SYSTEM/Attachments/img16.b459881e.jpg` | high | 제안 |

## Review-needed 항목

아래 항목은 이동 제안을 확정하지 않는다.

- `.DS_Store`, `.obsidian/.DS_Store`, `Work/.DS_Store`: 이동보다 gitignore/삭제 여부 확인이 먼저 필요하다.
- `Arkive/26.04 서사축.md`: 내용이 매우 짧아 임시 메모인지 자료인지 판단 불가.
- `Work/민족자결주의자를 위한 AI기술 활용/무제.md`: 제목과 역할이 불명확하다.
- `무제.base` 및 `무제 1.base`부터 `무제 6.base`: Bases 파일로 보이나 제목이 모두 임시 상태라 50_MAPS 이동 전 이름/역할 확인이 필요하다.
- `.obsidian` 전체: PARA상 90_SYSTEM 성격이지만 실제 파일 이동은 Obsidian 작동을 깨뜨릴 수 있으므로 현재 위치 유지.

## 다음 단계 제안

1. `review-needed` 항목의 역할을 사람이 확정한다.
2. 먼저 폴더만 만들고 파일 이동은 하지 않는 dry-run 스크립트를 만든다.
3. 첨부파일 이동은 Obsidian 링크 업데이트 전략을 먼저 정한다.
4. 일반 노트 이동 전 현재 Wikilink가 제목 기반으로 유지되는지 확인한다.
5. 이동 실행은 한 번에 하지 말고 `90_SYSTEM`, `10_PROJECTS`, `30_RESOURCES`, `40_ARCHIVES` 순서로 작은 커밋 단위로 나눈다.
