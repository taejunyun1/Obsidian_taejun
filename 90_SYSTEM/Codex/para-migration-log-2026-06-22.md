# PARA Migration Log

작성일: 2026-06-22

## 기준

- 적용 규칙: `AGENTS.md`
- 참조 분류표: `90_SYSTEM/Codex/para-migration-map.md`
- 실행 방식: 파일명 변경 없이 폴더 이동만 수행
- 원본 노트 본문 수정: 없음
- 새 내부링크 삽입: 없음
- 파일 삭제: 없음

## 선행 작업

- 이동 전 체크포인트 커밋을 `origin/main`에 푸시함.
- 커밋: `e205f17 Add vault rules and PARA migration map`

## 이동한 묶음

| 대상 | 이동 후 위치 | 비고 |
| --- | --- | --- |
| 빈/임시 키워드 노트 | `00_INBOX` | 빈 노트 1개 |
| 현재 진행 프로젝트 | `10_PROJECTS` | Transmitter to Object, 자결의 프로토콜, 접촉화면, 한미사진미술관, 논문, Le Wonder |
| 장기 협업 영역 | `20_AREAS` | 프로토콜 콜렉티브 날짜 기록 |
| 참고 자료 | `30_RESOURCES` | 작가, 이론/주제, 작업 레퍼런스, 제작기술 |
| 비활성/과거 기록 | `40_ARCHIVES` | 과거 질문, 광비 GB토크 |
| 첨부파일 | `90_SYSTEM/Attachments` | 이미지/첨부파일 57개 |
| Codex 운영 문서 | `90_SYSTEM/Codex` | cleanup 보고서, 링크 제안, migration map, 트러블슈팅 |
| 빈 기존 폴더 | 해당 없음 | 파일 이동 후 비어 있는 legacy 폴더만 제거함. 파일 삭제 없음 |

## 이동하지 않은 항목

아래 항목은 `AGENTS.md` 규칙상 확신이 낮거나 민감 확인이 필요해서 이동하지 않았다.

| 현재 경로 | 이유 |
| --- | --- |
| `Arkive/26.04 서사축.md` | 내용이 매우 짧아 임시 노트인지 참고 자료인지 판단 불가 |
| `Arkive/호반/교육프로그램.md` | 교육/참여자 맥락 가능성이 있어 사용자 확인 필요 |
| `Work/민족자결주의자를 위한 AI기술 활용/무제.md` | 제목과 역할이 불명확함 |
| `무제.base`, `무제 1.base` - `무제 6.base` | Bases 파일로 보이나 제목/역할 확인 필요 |
| `.DS_Store`, `.obsidian/.DS_Store`, `Work/.DS_Store` | 시스템 부산물로 삭제/추적 여부 확인 필요 |
| `.obsidian/**` | Obsidian 작동 파일이므로 이동 금지 |
| `.gitignore` | Git 운영 파일이므로 루트 유지 |
| `AGENTS.md` | Vault 운영 규칙이므로 루트 유지 |

## 후속 확인 필요

- `review-needed` 항목의 실제 성격 확정
- Obsidian에서 첨부파일 임베드 렌더링 확인
- `![[파일명\|숫자]]` 형식의 escaped pipe 임베드 확인
- 필요하면 `50_MAPS`에 MOC/Bases 정리 작업 별도 수행
