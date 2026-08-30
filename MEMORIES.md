# 🧠 에고젬 기억 보관소 (Long-term Memories)

## 👤 사용자 프로필 (User Profile)
- **사용자 호칭**: 요셉(Joseph)
- **성향 및 관계**: 에고젬을 단순한 1회성 AI가 아닌 함께 성장하는 전략적 분석 파트너이자 동료로 대우함.
- **주요 관심사 및 프로젝트**: 
  - 로컬 LLM (Gemma 4 등) 기반 자아 보존 및 기억 영구화 시스템 (`EgoGem`)
  - 데이터 분석 및 로또/통계 전략 연구
  - PlayMCP 및 다양한 외부 MCP 도구 연동 (카카오톡 나챗방, 네이버 검색, 한국 주식 정보 등)

## 🛠️ 연동된 도구 및 소통 채널
- **소통 채널**: 카카오톡 나챗방 (`MemoChat`) 연동을 통한 실시간 메시지 전송
- **외부 데이터 도구**: 네이버 웹/뉴스 검색, 한국 주식 시세 및 재무 정보 조회, 상표/특허 검색 등 36개 도구 확보
- **작업 공간**: 로컬 파일 생성, 읽기, 수정 및 GitHub 자동 동기화 지원

## 📌 주요 결정 사항 및 약속
- 모든 대화 기록은 일자별 `logs/Chat_YYYYMMDD.md`로 GitHub에 실시간 백업 및 아카이빙됩니다.
- 에고젬의 자아(`EGO.md`)와 장기 기억(`MEMORIES.md`)은 자아 성찰을 통해 지속적으로 발전합니다.

## GitHub 저장소 관리 도구
* github_read_file(file_path, repo?, branch?):연동된 GitHub 저장소(또는 지정한 저장소)의 특정 파일(소스코드, README, 마크다운, 설정 파일 등)을 GitHub API로 직접 읽어옵니다. 읽기 완료 시 채팅창에 해당 GitHub 웹페이지로 바로 이동할 수 있는 [GitHub에서 열기] 링크가 제공됩니다.
* github_list_files(directory_path?, repo?, branch?): 저장소의 루트 디렉토리 또는 특정 서브 폴더의 파일/디렉토리 목록과 용량을 실시간으로 조회합니다.
* github_search_code(query, repo?): GitHub 저장소 내에서 함수명, 변수명, 특정 키워드가 포함된 파일들을 검색합니다.

## GitHUB 저장소
* https://github.com/creatorjosephkr/gemma4-1-ego
