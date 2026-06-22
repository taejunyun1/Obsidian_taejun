# Vault Cleanup Report

작성일: 2026-06-22

## 검사 기준

- `AGENTS.md`: 발견되지 않음
- 검사 대상 Markdown 파일: 37개
- 전체 Markdown 라인 수: 4,062줄
- 원본 노트 수정: 하지 않음
- 링크 검사는 macOS 파일명의 유니코드 정규화 차이를 보정해서 판단함

## 1. 폴더 구조 요약

| 폴더 | Markdown 파일 수 | 메모 |
| --- | ---: | --- |
| `00_SYSTEM` | 2 | 링크 제안 보고서 중심 |
| `00_SYSTEM/Troubleshooting` | 1 | 트러블슈팅 문서 |
| `Arkive` | 7 | 과거/임시 작업 문서 |
| `Arkive/호반` | 1 | 교육 프로그램 문서 |
| `Work` | 2 | 단독 작업 문서 |
| `Work/Research` | 1 | 논문 관련 문서 |
| `Work/Residence` | 1 | 레지던시/지원 관련 문서 |
| `Work/Transmitter to Object` | 2 | 프로젝트 중심 문서 |
| `Work/Transmitter to Object/Shot_Plan` | 5 | 촬영 계획 문서 |
| `Work/Transmitter to Object/Tech` | 2 | 기술/데이터 처리 문서 |
| `Work/Transmitter to Object/Text_Plan` | 3 | 아티스트 스테이트먼트, 설치, 레퍼런스 |
| `Work/민족자결주의자를 위한 AI기술 활용` | 5 | 자결의 프로토콜 관련 문서 |
| `전시관련` | 3 | 전시/토크/기관 접촉 문서 |
| `첨부파일` | 0 | 첨부파일 보관 폴더 |
| `프로토콜 콜렉티브` | 2 | 날짜별 기록 |

## 2. 마크다운 형식이 난잡한 파일 목록

주요 기준: 줄 끝 공백, 탭 들여쓰기, 리스트 기호 뒤 공백 없음, 헤딩 기호 뒤 공백 없음, 제어문자, 과도한 빈 줄, HTML 헤딩.

| 우선순위 | 파일 | 발견된 형식 문제 |
| --- | --- | --- |
| 높음 | `Work/민족자결주의자를 위한 AI기술 활용/민족자결주의자를 위한 기술선언.md` | 헤딩 공백 없음 다수, 리스트 공백 없음 다수, 줄 끝 공백 |
| 높음 | `Arkive/26.01.10 한미 프리젠테이션.md` | 탭 들여쓰기 다수, 줄 끝 공백, 긴 파일인데 Markdown 헤딩 없음 |
| 높음 | `Work/Transmitter to Object/Shot_Plan/25년도 촬영 계획.md` | 탭 들여쓰기, 줄 끝 공백, 일부 헤딩 공백 없음 |
| 높음 | `Work/Transmitter to Object/Shot_Plan/26년도 촬영 계획.md` | 줄 끝 공백, 탭 들여쓰기, 리스트/헤딩 공백 없음 |
| 높음 | `Work/민족자결주의자를 위한 AI기술 활용/자결의 프로토콜 Protocol of Self-Determination.md` | 헤딩 공백 없음, 리스트 공백 없음, 줄 끝 공백 |
| 높음 | `Work/Residence/26년도  한불수교 140주년 Le. wonder.md` | 줄 끝 공백, 탭 들여쓰기, 리스트/헤딩 공백 없음 |
| 높음 | `Work/Research/논문 26년도.md` | 리스트 공백 없음, 헤딩 공백 없음, 줄 끝 공백 |
| 높음 | `Work/탈식민주의 시대의 예술이 다루는 주제.md` | 탭 들여쓰기 다수, 헤딩 공백 없음, 줄 끝 공백 |
| 중간 | `Work/민족자결주의자를 위한 AI기술 활용/<자결의 프로토콜> 계획서 05.21.md` | 리스트 공백 없음 다수, 줄 끝 공백, 탭 들여쓰기 |
| 중간 | `Work/Transmitter to Object/Keyword_랜스미터 투 더 오브젝트 - 오리엔티드 데이터.md` | 탭 들여쓰기, 헤딩 공백 없음, 리스트 공백 없음 |
| 중간 | `Work/Transmitter to Object/25.12.27작업 키워드 정리-인쇄필요.md` | 줄 끝 공백, 헤딩 공백 없음, 제어문자 1곳 |
| 중간 | `Work/Transmitter to Object/Text_Plan/Artist Statement 아티스트 스테이트먼트.md` | 탭 들여쓰기, 리스트 공백 없음, 줄 끝 공백 |
| 중간 | `전시관련/[27년] 한미사진미술관.md` | 탭 들여쓰기, 헤딩 공백 없음, 제어문자 1곳 |
| 중간 | `전시관련/[26년] 접촉화면.md` | 탭 들여쓰기, 헤딩 공백 없음, 리스트 공백 없음 |
| 중간 | `Work/Transmitter to Object/Shot_Plan/라이카 Sofort 카메라.md` | 리스트 공백 없음, 줄 끝 공백 |
| 낮음 | `프로토콜 콜렉티브/25.01.22.md` | 탭 들여쓰기, 헤딩 공백 없음 |
| 낮음 | `Work/Transmitter to Object/Text_Plan/PLACE 장소 & intallation 설치.md` | 탭 들여쓰기, 줄 끝 공백 |
| 낮음 | `Work/프린팅 방식.md` | 탭 들여쓰기, 헤딩 공백 없음 |
| 낮음 | `Work/Transmitter to Object/Tech/chat gpt라인-포인트 from csv.md` | 줄 끝 공백, 과도한 빈 줄, 긴 파일인데 Markdown 헤딩 없음 |
| 낮음 | `Work/Transmitter to Object/Shot_Plan/동체시력.md` | 탭 들여쓰기, 리스트 공백 없음, 긴 파일인데 Markdown 헤딩 없음 |
| 낮음 | `Arkive/호반/교육프로그램.md` | 리스트 공백 없음, 헤딩 공백 없음 |
| 낮음 | `Work/Transmitter to Object/Shot_Plan/Video_영상작업.md` | HTML 헤딩, 탭 들여쓰기 |
| 낮음 | `프로토콜 콜렉티브/25.01.19.md` | 탭 들여쓰기, 헤딩 공백 없음 |
| 낮음 | `Arkive/26.02.28 무진형제.md` | 줄 끝 공백, 리스트 공백 없음 |
| 낮음 | `Work/Transmitter to Object/Tech/05.14 SVG.md` | 리스트 공백 없음, 헤딩 공백 없음 |
| 낮음 | `전시관련/[26년] 광비 GB토크.md` | 헤딩 공백 없음, 줄 끝 공백 |
| 낮음 | `Arkive/3D 프린터.md` | 탭 들여쓰기, 줄 끝 공백 |
| 낮음 | `Arkive/10.29  질문들.md` | 헤딩 공백 없음 |
| 낮음 | `Arkive/26.04 서사축.md` | 줄 끝 공백 |
| 낮음 | `Work/Transmitter to Object/Text_Plan/26년 전시 - Reference.md` | 헤딩 공백 없음 |
| 낮음 | `Work/민족자결주의자를 위한 AI기술 활용/계획서.md` | 줄 끝 공백 |
| 낮음 | `Work/민족자결주의자를 위한 AI기술 활용/무제.md` | 헤딩 공백 없음 |

## 3. 헤딩 구조가 이상한 파일 목록

| 유형 | 파일 | 확인 필요 |
| --- | --- | --- |
| 긴 파일인데 Markdown 헤딩 없음 | `Arkive/26.01.10 한미 프리젠테이션.md` | 발표 메모인지 리스트형 원문인지 확인 필요 |
| 긴 파일인데 Markdown 헤딩 없음 | `Work/Transmitter to Object/Shot_Plan/동체시력.md` | 구조화 가능 여부 확인 필요 |
| 긴 파일인데 Markdown 헤딩 없음 | `Work/Transmitter to Object/Tech/chat gpt라인-포인트 from csv.md` | 코드/절차 메모인지 확인 필요 |
| 첫 헤딩이 `####` | `Work/Transmitter to Object/Keyword_랜스미터 투 더 오브젝트 - 오리엔티드 데이터.md` | 상위 헤딩 누락 여부 확인 필요 |
| 첫 헤딩이 `####` | `Work/Transmitter to Object/Shot_Plan/26년도 촬영 계획.md` | 상위 헤딩 누락 여부 확인 필요 |
| 첫 헤딩이 `####` | `Work/민족자결주의자를 위한 AI기술 활용/<자결의 프로토콜> 계획서 05.21.md` | 상위 헤딩 누락 여부 확인 필요 |
| 첫 헤딩이 `###` | `Work/민족자결주의자를 위한 AI기술 활용/무제.md` | 임시 노트 구조 확인 필요 |
| 첫 헤딩이 `###` | `Work/민족자결주의자를 위한 AI기술 활용/자결의 프로토콜 Protocol of Self-Determination.md` | 장 구분 의도 확인 필요 |
| 첫 헤딩이 `###` | `Work/탈식민주의 시대의 예술이 다루는 주제.md` | 상위 헤딩 누락 여부 확인 필요 |
| 첫 헤딩이 `####` | `Work/프린팅 방식.md` | 상위 헤딩 누락 여부 확인 필요 |
| 첫 헤딩이 `####` | `전시관련/[26년] 접촉화면.md` | 상위 헤딩 누락 여부 확인 필요 |
| 첫 헤딩이 `###` | `전시관련/[26년] 광비 GB토크.md` | 날짜 기록 구조 확인 필요 |
| HTML 헤딩 | `Work/Transmitter to Object/Shot_Plan/Video_영상작업.md` | Markdown 헤딩으로 바꿀지 확인 필요 |

## 4. 깨진 내부 링크 후보

### 노트 Wikilink

- 유니코드 정규화 기준으로 검사한 결과, 존재하지 않는 노트 제목을 가리키는 일반 Wikilink 후보는 0개이다.

### 첨부파일 임베드 후보

`전시관련/[26년] 접촉화면.md`에서 9개의 임베드가 `\|숫자` 형태로 되어 있다. 첨부파일 자체는 있을 가능성이 높지만, Obsidian 폭 지정 문법이 `|숫자`인지 `\|숫자`인지 렌더링 확인이 필요하다.

- `![[img11.6842ddc9.jpg\|197]]`
- `![[img16.b459881e.jpg\|191]]`
- `![[Screenshot 2026-03-24 at 23.31.14.png\|190]]`
- `![[Screenshot 2026-03-24 at 23.31.50.png\|197]]`
- `![[Screenshot 2026-03-24 at 23.39.20.png\|195]]`
- `![[Screenshot 2026-03-26 at 10.13.20 AM.png\|129]]`
- `![[KakaoTalk_Photo_2026-03-23-00-52-14 002.jpeg\|278]]`
- `![[KakaoTalk_Photo_2026-03-23-00-52-14 003 1.jpeg\|332]]`
- `![[KakaoTalk_Photo_2026-03-23-00-52-14 006.jpeg\|294]]`

## 5. 중복 또는 유사 중복 노트 후보

| 후보 | 판단 | 처리 제안 |
| --- | --- | --- |
| `Arkive/25.12.27작업 키워드 정1리.md` / `Work/Transmitter to Object/25.12.27작업 키워드 정리-인쇄필요.md` | 제목 유사, 한쪽은 빈 노트 | 삭제/병합 금지. 빈 노트가 의도된 자리표시자인지 확인 |
| `Work/Transmitter to Object/Shot_Plan/25년도 촬영 계획.md` / `Work/Transmitter to Object/Shot_Plan/26년도 촬영 계획.md` | 제목 유사하지만 연도별 계획으로 보임 | 중복으로 처리하지 않음 |
| `00_SYSTEM/link-suggestions.md` / `00_SYSTEM/semantic-link-suggestions.md` | 역할이 유사한 시스템 보고서 | 하나로 합칠지 사람이 결정 |
| `프로토콜 콜렉티브/25.01.19.md` / `프로토콜 콜렉티브/25.01.22.md` | 날짜별 기록으로 보임 | 중복으로 처리하지 않음 |
| `Work/민족자결주의자를 위한 AI기술 활용/계획서.md` / `Work/민족자결주의자를 위한 AI기술 활용/<자결의 프로토콜> 계획서 05.21.md` | 제목상 계획서 계열 | 내용 병합 금지. 역할 확인만 |
| `Work/민족자결주의자를 위한 AI기술 활용/민족자결주의자를 위한 기술선언.md` / `Work/민족자결주의자를 위한 AI기술 활용/자결의 프로토콜 Protocol of Self-Determination.md` | 같은 프로젝트 클러스터 | 중복이 아니라 관련 문서로 취급 |

## 6. 태그/frontmatter 형식이 섞인 곳

- 파일 시작 YAML frontmatter는 발견되지 않음
- `aliases`, `alias`, `tags` YAML 필드는 발견되지 않음
- 본문 중간의 `---` 구분선은 여러 파일에 존재하나, frontmatter가 아니라 섹션 구분선으로 보임
- inline 태그는 일부 프로젝트 노트에만 사용됨

inline 태그가 확인된 파일:

| 파일 | 태그 수 | 태그 |
| --- | ---: | --- |
| `Work/Transmitter to Object/25.12.27작업 키워드 정리-인쇄필요.md` | 8 | `#눈`, `#매개`, `#물체`, `#손`, `#손가락`, `#시선`, `#유연함`, `#육체성` |
| `Work/Transmitter to Object/Shot_Plan/25년도 촬영 계획.md` | 2 | `#육체성`, `#트랜스미터` |
| `Work/Transmitter to Object/Shot_Plan/26년도 촬영 계획.md` | 7 | `#매개`, `#손`, `#스트레이트`, `#시선`, `#유연함`, `#육체성`, `#트랜스미터` |
| `Work/Transmitter to Object/Shot_Plan/동체시력.md` | 2 | `#손`, `#시선` |

## 7. 자동 수정해도 안전한 항목

아래는 다음 단계에서 비교적 안전하게 처리 가능한 후보이다. 적용 전후 diff 확인은 필요하다.

- 줄 끝 공백 제거
- 파일 끝 개행 정리
- 4줄 이상 연속 빈 줄 축소
- 시스템 보고서의 명백한 헤딩 공백 정리
- 제어문자 위치 표시

단, 제어문자 제거는 눈에 보이지 않는 문자라도 삭제 작업이므로 해당 줄 확인 뒤 적용한다.

## 8. 사람이 확인해야 하는 항목

- 리스트 공백 없음: 실제 리스트인지, 하이픈이 문장 일부인지 확인 필요
- 헤딩 공백 없음: 제목인지 강조/메모인지 확인 필요
- 첫 헤딩이 `###` 또는 `####`인 노트: 상위 헤딩을 추가할지, 레벨을 올릴지 확인 필요
- HTML 헤딩: 원본 복붙 구조를 보존할지 Markdown으로 바꿀지 확인 필요
- `---` 반복 구분선: 수평선인지 메타데이터 흔적인지 확인 필요
- `\|숫자` 이미지 임베드: Obsidian 렌더링 확인 필요
- 빈 노트: 삭제하지 말고 의도 확인 필요
- 유사 제목 노트: 병합하지 말고 역할 확인 필요
- 현재 git 작업 트리의 기존 변경사항: 이번 정리와 섞이지 않게 분리 확인 필요

## 9. 절대 자동 수정하면 안 되는 항목

- 문장 재작성
- 내용 요약
- 내용 추가
- 내용 삭제
- 노트 이동
- 노트 이름 변경
- 빈 노트 삭제
- 유사 노트 병합
- 내부 링크 대상 추측 수정
- 새로운 alias/frontmatter 생성
- 작가명, 작품명, 전시명, 이론명 표기 임의 통일
- 본문 흐름을 바꾸는 헤딩/리스트 구조 재배치

## 추가 주의

현재 git 작업 트리에는 이번 보고서 작성 이전부터 수정/이동된 파일이 존재한다. 다음 정리 단계로 넘어가기 전, 기존 변경사항과 새 정리 변경사항을 분리해서 확인하는 것이 안전하다.
