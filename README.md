# CursorLingo

**마우스 커서 주변 텍스트를 자동으로 감지하고 즉시 번역해주는 데스크탑 앱**

> 단축키 하나로, 마우스가 가리키는 텍스트를 자동으로 인식하고 번역 결과를 팝업으로 보여줍니다.

---

## 주요 기능

### 커서 기반 자동 번역
`Alt + T`를 누르면 현재 마우스 커서 위치에서 가장 가까운 텍스트를 자동으로 탐지합니다.
- **단어** — 커서 바로 아래 단어 하나
- **문장** — 구두점 기준으로 감지된 전체 문장
- **문단** — 의미 단위로 묶인 텍스트 블록

화면 어디서든 동작합니다. 브라우저, PDF, 게임, 영상 자막 모두 지원.

### 드래그 영역 선택
마우스로 드래그해서 원하는 영역을 직접 지정하면 해당 영역의 텍스트만 인식해서 번역합니다.

### 번역 엔진 선택
| 엔진 | 특징 |
|------|------|
| **Google Translate API** | 빠른 속도, 다양한 언어 지원 |
| **Gemma Translate 4B** (LLM) | 로컬 실행, 인터넷 연결 불필요, 문맥 기반 번역 |

---

## 다운로드

[**Releases 페이지**](../../releases)에서 운영체제에 맞는 파일을 받으세요.

| 운영체제 | 파일 |
|----------|------|
| macOS (Apple Silicon) | `CursorLingo-x.x.x.dmg` |
| Windows | `CursorLingo-x.x.x-setup.exe` |
| Linux | `CursorLingo-x.x.x.AppImage` |

---

## 설치 방법

### macOS
1. `.dmg` 파일을 열고 `CursorLingo.app`을 `/Applications`로 드래그
2. 처음 실행 시 Gatekeeper 차단 경고가 나타납니다. 아래 중 하나로 해결하세요:

   **방법 A** — Finder에서 앱 우클릭 → **열기** → 경고창에서 **열기** 클릭

   **방법 B** — 터미널에서 실행:
   ```bash
   xattr -dr com.apple.quarantine /Applications/CursorLingo.app
   ```

3. 시스템 환경설정 → **개인 정보 보호 및 보안** → **화면 녹화** → CursorLingo 허용

### Windows
1. `.exe` 설치 파일 실행
2. SmartScreen 경고가 나타나면 **추가 정보** → **실행** 클릭

### Linux
```bash
chmod +x CursorLingo-x.x.x.AppImage
./CursorLingo-x.x.x.AppImage
```

---

## 사용 방법

1. 앱 실행 후 번역 엔진 선택 (설정 화면)
2. 번역할 텍스트가 있는 화면 위로 마우스 이동
3. `Alt + T` → 커서 주변 텍스트 자동 감지 및 번역 팝업 표시
4. 또는 드래그로 영역을 선택한 뒤 `Alt + T`

---

## 시스템 요구 사항

| | 최소 사양 |
|-|-----------|
| **macOS** | 13 Ventura 이상 (Apple Silicon) |
| **Windows** | Windows 10 이상 (x64) |
| **Linux** | Ubuntu 20.04 이상 |

LLM 번역(Gemma 4B) 사용 시 별도의 번역 서버 실행이 필요합니다.

---

## 라이선스

MIT License
