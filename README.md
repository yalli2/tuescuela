# Tu escuela de español — 영상 검색 사이트

유튜브 채널 [**Tu escuela de español**](https://www.youtube.com/@tuescueladeespanoles) (Elena Prieto, 구독자 51.6만 · 영상 386편)의
강의 영상을 **주제·레벨별로 검색해 사이트 안에서 바로 시청**할 수 있는 검색 도구입니다.

🔗 **사이트:** https://yalli2.github.io/tuescuela/

---

## 기능

| 기능 | 설명 |
|---|---|
| 🔍 **즉시 검색** | 제목·설명을 악센트 무시(`subjuntivo` = `subjuntívo`)로 검색, 여러 단어 AND 조건 |
| 🎚 **레벨 필터** | básico / intermedio / avanzado — 제목의 `(nivel …)` 표기를 자동 인식 |
| 🏷 **주제 필터** | 문법 · 어휘 · 동사 · 발음 · 표현 · 문화 · 시험 — 스페인어 키워드 규칙으로 자동 분류 |
| ▶️ **인라인 재생** | 카드 클릭 → 사이트 내 모달에서 스페인어 자막 자동 ON으로 재생 |
| ↕️ **정렬** | 정확도 · 최신 · 오래된 · 조회수순 |
| 🎲 **랜덤 영상** | 현재 필터 안에서 무작위 추천 (수업 도입용) |
| 🌐 **3개 언어** | 한국어 / Español / English 인터페이스 전환 |
| ⌨️ **단축키** | `/` 검색창 포커스, `Esc` 플레이어 닫기 |

---

## 전체 386편 검색 활성화 (무료, 1회)

유튜브는 외부 사이트가 채널의 영상 목록을 직접 읽는 것을 허용하지 않습니다.
구글이 **무료로** 제공하는 YouTube Data API 키를 한 번만 등록하면, 사이트가 전체 목록을
받아 브라우저에 저장하고 **그 뒤로는 서버 호출 없이 즉시** 검색됩니다.

1. [Google Cloud Console](https://console.cloud.google.com/projectcreate)에서 새 프로젝트 생성
2. [YouTube Data API v3](https://console.cloud.google.com/apis/library/youtube.googleapis.com) → **사용** 클릭
3. [사용자 인증 정보](https://console.cloud.google.com/apis/credentials) → **사용자 인증 정보 만들기** → **API 키**
4. 사이트 하단 ⚙️ 패널에 키(`AIza…`) 붙여넣기 → **저장하고 불러오기**

**보안**
- 키는 **방문자 각자의 브라우저 localStorage**에만 저장됩니다. 저장소에 커밋되지 않고 외부 서버로도 전송되지 않습니다.
- 구글 콘솔에서 키 제한을 **HTTP 리퍼러** → `https://yalli2.github.io/*` 로 걸어두면 더 안전합니다.
- 전체 목록 1회 수신에 드는 할당량은 약 **8 단위** (무료 일일 한도 10,000 단위).

### 키 없이 쓸 때 (맛보기 모드)
키를 등록하지 않아도 다음은 그대로 작동합니다.
- 조회수 상위 대표 영상 카드와 재생
- **채널 전체 재생목록** 플레이어 (업로드 386편 전체 순차 재생)
- 입력한 검색어 그대로 **유튜브 채널 내 검색**으로 바로 이동

---

## 수업 활용 팁

- 수업 전 `subjuntivo`, `ser y estar`, `por y para` 처럼 그날 문법을 검색해 **레벨 필터**로 좁히면 학생 수준에 맞는 영상만 남습니다.
- **🎲 랜덤 영상**을 `어휘` + `básico`로 걸어두면 수업 도입 듣기 활동으로 쓸 수 있습니다.
- 플레이어는 스페인어 자막(`cc_lang_pref=es`)이 기본 ON이라 받아쓰기·섀도잉에 바로 쓸 수 있습니다.

---

## 배포

GitHub Pages — **Settings → Pages → Source: `main` / `(root)`**

의존성 없는 단일 `index.html` 파일입니다. 빌드 과정이 없습니다.

---

## 저작권

비공식 검색 도구입니다. 모든 영상의 저작권과 소유권은 채널 운영자
**Elena Prieto (Tu escuela de español)** 에게 있습니다.
이 사이트는 영상을 저장하거나 재배포하지 않으며, 재생은 전부 유튜브 공식
임베드 플레이어(`youtube-nocookie.com`)를 통해 이루어집니다.

제작: **다인에듀 (후안샘)** · [dainedu.net](https://www.dainedu.net)
