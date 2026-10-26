# AI_illustLab

일러스트 생성용 작업 공간. 요청을 받으면 아래 규칙을 따른다.

## 라우팅
- 캐릭터가 등장하는 그림 요청 → `.agents/skills/character-illust/SKILL.md`를 읽고 그 절차를 따른다.
- 소품·아이템·무기·장신구의 설정화 요청 → `.agents/skills/prop-design/SKILL.md`를 읽고 그 절차를 따른다.

## 폴더
- `confirmed/README.md`: 확정 디자인 목록. 작업 전 해당 항목을 확인한다.
- `confirmed/characters/<이름>/`: 기준 이미지 `design.png` 또는 `design.jpeg`, 확정 기록 `design.md`, 상세 설정 `settings.md`(있는 경우).
- `confirmed/props/<이름>/`: 기준 이미지·확정 기록·소품 상세 설정 `settings.md`.
- `confirmed/styles/`: 확정 디자인을 사용하는 데 필요한 스타일 정의.
- `_archive/`: 확정본 외의 모든 작업 자료를 모은 로컬 보관 폴더. Git에서 제외한다.
- `_archive/outputs/`: 시안·이전 확정본·생성 프롬프트·검수 이력.
- `_archive/characters/`, `_archive/styles/`, `_archive/props/`, `_archive/refs/`, `_archive/requests/`: 이전 설정·원본 자료·양식·요청서.
- `_template.md`로 시작하는 파일은 양식일 뿐이니 생성에 쓰지 않는다.

## 스킬의 이전 경로 해석
- 스킬에 이전 폴더 경로가 나오면 아래 현재 경로를 우선 적용한다. `.agents/`는 실행 지침으로 유지한다.
- 캐릭터 설정은 `confirmed/characters/<이름>/design.md`와 `settings.md`(있는 경우), 소품 설정은 `confirmed/props/<이름>/settings.md`를 읽는다.
- 스타일은 `confirmed/styles/<스타일>.md`, 기준 이미지는 해당 확정 폴더의 `design.png` 또는 `design.jpeg`를 사용한다.
- 요청서는 `_archive/requests/`에서 찾고, 없으면 사용자 메시지를 따른다. 템플릿은 `_archive/`의 이전 종류별 폴더에서 찾는다.
- 스킬의 `outputs/` 저장 및 `refs/` 확정 복사 절차 대신 아래 공통 규칙을 따른다.

## 공통 규칙
- 결과는 `_archive/outputs/YYYY-MM-DD_<요청명>/`에 저장한다.
  - 이미지: `01.png`, `02.png` …
  - 최종 프롬프트와 설정: `prompt.md` (사용한 캐릭터/스타일 파일, 최종 프롬프트 원문, 네거티브, 비율, 시도별 수정 내역)
- 설정 파일에 없는 외형을 지어내지 않는다. 정보가 부족하면 먼저 질문한다.
- 외형·스타일·소품 설정 내용은 사용자가 요청할 때만 수정한다.
- 기존 캐릭터·소품의 작업 전 `confirmed/README.md`에서 확정 디자인을 확인하고 해당 `design.md`와 기준 이미지를 참조한다.
- 사용자가 새 버전을 확정하면 `confirmed/`의 해당 기준 이미지·기록·목록을 갱신한다. 이전 결과와 프롬프트는 `_archive/outputs/`에 보존한다. 시안 생성만으로 확정본을 바꾸지 않는다.
- 확정 기록의 `_archive/` 링크는 이력 조회용이다. 현재 디자인은 `confirmed/`만으로 확인할 수 있어야 한다.
