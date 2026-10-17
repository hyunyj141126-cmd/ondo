# Ondo AI

모바일 게임 만들기를 도와주는 AI입니다. 휴대폰 안에서 직접 돌아가서 계정, API 키, 서버가 필요 없습니다.
An AI helper for making mobile games. It runs on your phone, so you don't need an account, an API key, or a server.

---

## 한국어

### 이 폴더에 든 파일

| 파일 | 하는 일 |
|---|---|
| `index.html` | Ondo 앱 본체 |
| `manifest.webmanifest` | 홈 화면에 앱으로 설치할 때 쓰는 정보 |
| `sw.js` | 인터넷이 없어도 앱이 열리게 해 주는 파일 |
| `icon-*.png`, `icon.svg`, `apple-touch-icon.png` | 앱 아이콘 |

파일 이름과 위치를 바꾸지 말고, 폴더 안의 파일을 **전부 함께** 올려 주세요.

### 인터넷에 올리는 방법 (무료)

**방법 1. GitHub Pages**

1. github.com에 가입하고 로그인합니다.
2. 오른쪽 위 **+** → **New repository**를 누르고, 이름(예: `ondo`)을 정한 뒤 **Public**으로 만듭니다.
3. 새 저장소 화면에서 **Add file → Upload files**를 누르고, 이 폴더 안의 파일을 모두 끌어다 놓은 뒤 **Commit changes**를 누릅니다.
4. **Settings → Pages**로 가서 **Source**를 **Deploy from a branch**로, 브랜치를 **main**, 폴더를 **/ (root)**로 고르고 **Save**를 누릅니다.
5. 1~2분 뒤 `https://내아이디.github.io/ondo/` 주소로 열립니다.

**방법 2. Netlify**

1. app.netlify.com/drop 에 접속합니다.
2. 이 폴더를 통째로 화면에 끌어다 놓으면 바로 주소가 생깁니다. 사이트를 계속 유지하려면 로그인하라는 안내가 나올 수 있습니다.

주소는 꼭 **https://** 로 시작해야 합니다. 그래야 휴대폰 안에서 AI가 돌아가고, 앱 설치와 오프라인 사용도 됩니다.

### 휴대폰에서 쓰는 방법

1. 올린 주소를 휴대폰에서 엽니다. 안드로이드는 최신 **Chrome**, 아이폰은 **iOS 26 이상**의 **Safari**를 쓰세요.
2. 처음 질문하면 AI 모델을 한 번 받습니다. **‘기본’ 모델은 약 1.1GB**이니 와이파이에서 받으세요.
3. 받은 뒤로는 인터넷 없이도 답합니다.
4. **설정 → 앱으로 설치**를 누르면 홈 화면에 아이콘이 생깁니다. 아이폰은 Safari의 공유 버튼 → **홈 화면에 추가**를 누르세요.
5. **설정 → 언어**에서 English, 한국어, 日本語, 简体中文, Español 중에 고를 수 있습니다. 처음에는 영어로 시작합니다.

### 알아 두세요

- 휴대폰에 들어가는 작은 AI라서 틀린 답을 할 수 있습니다. 중요한 내용은 공식 문서로 확인하세요.
- 오래된 휴대폰은 메모리가 부족할 수 있습니다. 그럴 땐 **‘빠르게’ 모델(약 0.5GB)**을 고르세요.
- 대화 기록과 모델은 그 휴대폰에만 저장되고, 다른 곳으로 보내지지 않습니다.
- 처음 한 번은 인터넷에서 AI 엔진(jsDelivr)과 모델 파일(Hugging Face)을 받아 옵니다.

### 앱을 고친 뒤 다시 올릴 때

`sw.js` 맨 위의 `ondo-v1`을 `ondo-v2`처럼 숫자를 올려 주세요. 그래야 이미 설치한 휴대폰에도 새 버전이 들어갑니다.

---

## English

### What's in this folder

| File | What it does |
|---|---|
| `index.html` | The Ondo app |
| `manifest.webmanifest` | Info used when installing Ondo on the home screen |
| `sw.js` | Lets the app open without internet |
| `icon-*.png`, `icon.svg`, `apple-touch-icon.png` | App icons |

Upload **all** the files together, without renaming or moving them.

### Put it online (free)

**Option 1. GitHub Pages**

1. Sign up at github.com and sign in.
2. Click **+** (top right) → **New repository**, give it a name (e.g. `ondo`), and make it **Public**.
3. On the new repository page, click **Add file → Upload files**, drag in every file from this folder, and click **Commit changes**.
4. Go to **Settings → Pages**. Set **Source** to **Deploy from a branch**, branch **main**, folder **/ (root)**, then **Save**.
5. After a minute or two, open `https://YOUR-NAME.github.io/ondo/`.

**Option 2. Netlify**

1. Go to app.netlify.com/drop.
2. Drag this whole folder onto the page. You get a web address right away. You may be asked to sign in to keep the site online.

The address must start with **https://**. That's what lets the AI run on the phone, and makes installing and offline use work.

### Using it on a phone

1. Open your address on the phone. Use the latest **Chrome** on Android, or **Safari on iOS 26 or later** on iPhone.
2. Your first question downloads an AI model once. **The Standard model is about 1.1 GB**, so use Wi-Fi.
3. After that, Ondo answers without internet.
4. Tap **Settings → Install as an app** to add an icon to your home screen. On iPhone, tap Safari's Share button → **Add to Home Screen**.
5. Pick your language in **Settings → Language**: English, 한국어, 日本語, 简体中文 or Español. It starts in English.

### Good to know

- It's a small AI that fits on a phone, so it can be wrong. Double-check important things in the official docs.
- Older phones may run out of memory. If so, choose the **Quick model (about 0.5 GB)**.
- Chats and models are stored only on that phone and are not sent anywhere.
- The first time, it downloads the AI engine (from jsDelivr) and the model files (from Hugging Face).

### After you change the app

Bump `ondo-v1` at the top of `sw.js` (e.g. to `ondo-v2`) so phones that already installed Ondo get the new version.

### Try it on your computer (for developers)

Run a local web server in this folder, for example `python3 -m http.server 8080`, then open `http://localhost:8080`.

---

Credits: AI engine [WebLLM](https://github.com/mlc-ai/web-llm) (Apache-2.0). Models: Qwen3 and Qwen2.5-Coder by the Qwen team (Apache-2.0).
