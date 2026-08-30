현재 **에고젬(EgoGem)** 안에서 AI(Gemma 4:12b 등)가 직접 호출하여 실행할 수 있는 전체 도구 목록입니다. 🛠️

---

### 📂 1. 로컬 작업 공간(Workspace & Memory) 도구

| 도구 이름 | 설명 | 사용 예시 |
| :--- | :--- | :--- |
| **`create_file`** | `workspace/` 또는 `local_memory/`에 새 파일(코드, 문서, 스크립트) 생성 및 저장 | `file_path: "scraper.py"`, `content: "..."` |
| **`read_file`** | 로컬 작업공간 파일, 대화 로그(`logs/`), `EGO.md`, `MEMORIES.md` 내용 읽기 | `file_path: "workspace/hello.py"`, `file_path: "EGO.md"` |
| **`edit_file`** | 기존 파일 내의 특정 텍스트/코드 블록을 찾아 부분 수정 및 교체 | `file_path: "main.py"`, `search_text: "..."`, `replace_text: "..."` |
| **`delete_file`** | 로컬 작업 공간의 파일 삭제 | `file_path: "temp.txt"` |
| **`rename_file`** | 로컬 작업 공간 파일 이름 변경 | `file_path: "app.py"`, `new_name: "app_v2.py"` |
| **`list_directory`** | 작업 공간 디렉토리의 파일/폴더 목록 및 파일 크기 조회 | `directory: ""` (루트), `directory: "workspace"` |
| **`search_files`** | 로컬 작업 공간 및 메모리 폴더에서 파일명/내용 키워드 검색 | `query: "로또"`, `query: ".py"` |

---

### 🐙 2. GitHub 원격 저장소 직접 탐색 도구 *(New)*

연동된 GitHub 저장소(또는 임의의 GitHub 저장소)의 소스코드와 문서를 AI가 직접 읽고 탐색합니다.

| 도구 이름 | 설명 | 사용 예시 |
| :--- | :--- | :--- |
| **`github_read_file`** | GitHub 원격 저장소의 파일(소스코드, README, 설정 등) 직접 읽기 *(GitHub 바로가기 링크 제공)* | `file_path: "README.md"`, `file_path: "backend/app/main.py"` |
| **`github_list_files`** | GitHub 저장소의 루트 또는 특정 폴더 내 파일/디렉토리 트리 목록 조회 | `directory_path: ""`, `directory_path: "src"` |
| **`github_search_code`** | GitHub 저장소 내에서 함수명, 변수명, 키워드 검색 | `query: "stream_chat"`, `repo: "owner/repo"` |

---

### 🔌 3. MCP (Model Context Protocol) & 카카오 PlayMCP 도구

외부 서비스 및 실시간 API와 연동하여 동작하는 도구입니다.

| 도구 이름 | 설명 |
| :--- | :--- |
| **`get_current_time`** | 현재 날짜 및 시각을 실시간 조회 |
| **`mcp__kakaotalk_send`** | 카카오톡 나에게 보내기 / 메시지 전송 |
| **`mcp__google_calendar_create`** | 구글 캘린더에 새 일정 등록 |
| **`mcp__kakao_map_search`** | 카카오 지도 기반 주변 장소, 맛집, 위치 검색 |
| **`mcp__stock_price_inquiry`** | 실시간 국내/해외 주식 시세 및 주가 조회 |
| **사용자 등록 커스텀 MCP** | 설정에서 등록한 외부 MCP 서버의 도구들이 자동 추가 |

---

### 🌐 4. 실시간 웹 검색 (Web Search)

- **DuckDuckGo 실시간 웹 검색**: 채팅창의 **[🌐 웹 검색]** 토글이 켜져 있을 때, 최신 정보나 실시간 뉴스를 검색하여 답변에 자동으로 반영합니다.

---

### 💡 대화창에서 바로 활용하는 방법 예시
* *"내 깃허브 저장소에 있는 `README.md` 읽고 요약해줘"*
* *"작업 공간에 주식 차트를 그리는 파이썬 스크립트 파일 하나 만들어줘"*
* *"현재 시간 확인하고 오늘 할 일 일정 캘린더에 등록해줘"*
* *"깃허브 저장소의 `backend/app` 폴더에 파일 목록 뭐뭐 있어?"*