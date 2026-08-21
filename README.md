# 📚 DURU — 두루 돕는 AI

<div align="right">

**한국어** | [English](README.en.md)

</div>

> 연구 · 교육 · 업무를 두루 돕는, 내 PC 안의 AI 에이전트

---

<div align="center">
  <img src="assets/duru_intro.png" alt="DURU — 두루 돕는 AI" width="92%" />
</div>

---

> ## 📢 윈도우 설치판이 나왔습니다 — **v0.8.0**
>
> <sub>2026-08-21</sub>
>
> 설치 파일 하나(약 300MB)를 받아 실행하면 끝입니다. → **[내려받기](../../releases/latest)**
> **지식베이스가 이미 들어 있습니다** — 「국가 제도·법령 (표본 15편)」이 함께 설치되어,
> 처음 켜는 순간부터 물어볼 것이 있습니다. 따로 받아 넣지 않아도 됩니다.
>
> 🍎 **맥용도 곧 공개합니다.** 준비되는 대로 이 페이지에서 알려 드리겠습니다.

---

## 🔎 한눈에

DURU는 **내가 가진 문서를 근거로 답하는 AI**입니다.
클라우드 서비스가 아니라 내 PC에 설치해서 씁니다.

- 📄 **내 문서에서 답을 찾습니다** — 규정집·논문·교재를 넣어 두면, 질문할 때 그 안에서 근거를 찾아 **어느 문서 몇 쪽인지** 함께 알려 줍니다.
- 🔒 **자료가 밖으로 나가지 않습니다** — 문서도 AI 모델도 내 PC 안에 있습니다. **망분리된 내부망**에서도 씁니다.
- 📦 **한 번 만들어 함께 씁니다** — 담당자가 정리해 둔 지식베이스와 에이전트를 **파일로 받으면** 바로 쓸 수 있습니다.
- 💻 **설치가 전부입니다** — 서버도, 전용 그래픽카드도, 운영 담당자도 필요 없습니다.

---

## 🖥️ 이렇게 생겼습니다

<div align="center">
  <img src="assets/main-overview.png" alt="DURU 화면 — 왼쪽에 지식베이스와 문서 목록, 가운데에 문서 뷰어(근거가 상자로 표시됨), 오른쪽에 에이전트와 대화" width="94%" />
</div>

<sub>왼쪽은 **지식베이스**, 가운데는 **문서 뷰어**, 오른쪽은 **에이전트**입니다.
답변의 근거를 누르면 가운데 뷰어가 그 문서 그 위치로 이동하고, 인용된 대목이 상자로 표시됩니다.</sub>

---

## 📦 만들어 둔 것을 받아서 씁니다

준비 작업은 무겁습니다. 규정집 수백 권을 정리하려면 좋은 PC에서도 시간이 걸립니다.
그렇다고 구성원 100명이 각자 반복할 이유는 없습니다.

**담당자가 한 번 만들어 파일로 나눠 주면**, 받는 쪽은 가져오기만 하면 됩니다.
다시 계산하지 않고 **그 자리에서 바로** 검색됩니다.

<div align="center">
  <img src="assets/kb-import.png" alt="설정 화면의 지식베이스 목록 — 가져온 지식베이스의 문서 수와 조각 수가 보인다" width="88%" />
</div>

> [!NOTE]
> 직접 만들지 않아도 됩니다. **이미 만들어진 지식베이스를 파일로 받으면**
> 준비 과정 없이 그 자리에서 바로 쓸 수 있습니다.

---

## 👥 어디에 쓰나

| 분야 | 이런 상황 | DURU의 역할 |
| --- | --- | --- |
| 🏛️ 행정 | 규정·지침이 방대해 어디를 봐야 할지 막막할 때 | "이건 규정상 가능한가요?"에 **해당 조문**을 찾아 설명합니다 |
| 🔬 연구 | 논문·보고서 더미에서 필요한 대목을 찾아야 할 때 | 질문 한 번에 **근거 페이지까지** 짚어 줍니다 |
| 🎓 교육 | 수업 자료로 문제를 내거나, 학생이 혼자 공부할 때 | 교재로 퀴즈를 만들고, 쉽게 다시 설명합니다 |
| 💼 사무 | 문서 요약·초안 작성이 반복될 때 | 열려 있는 문서를 보며 요약과 초안을 돕습니다 |

---

## ✨ 주요 기능

### 🔍 근거를 짚어 주는 답변

일반 챗봇은 사실이 아닌 내용을 그럴듯하게 지어낼 수 있습니다.
규정을 다루는 자리에서 그건 도움이 아니라 사고입니다.

DURU는 **등록된 문서 안에서만** 근거를 찾아 답하고, 출처를 함께 보여줍니다.
답변 아래의 근거를 누르면 **원문의 그 자리로** 이동합니다. 맞는지 30초면 확인됩니다.
근거를 찾지 못하면 지어내지 않고 "확인되지 않는다"고 답하도록 되어 있습니다.

문서에서 문단·표·그림이 **어디에 있는지까지** 읽어 두기 때문에,
답변의 근거가 문서의 어느 위치인지 정확히 가리킬 수 있습니다.

<div align="center">
  <img src="assets/answer-evidence.png" alt="답변 아래에 근거가 문서 이름·쪽수·유사도와 함께 펼쳐진 모습" width="52%" />
</div>

<sub>실제 예 — *"국가공무원법에서 정한 징계의 종류는 무엇인가요?"* 에 **파면·해임·강등·정직·감봉·견책**이라 답하고,
근거 다섯 곳을 문서·쪽수와 함께 보여 줍니다. 오른쪽 백분율은 질문과 얼마나 가까운 대목인지입니다.</sub>

<div align="center">
  <img src="assets/evidence-in-page.png" alt="근거를 누르면 뷰어가 해당 쪽으로 이동하고 인용된 조문이 상자로 표시된다" width="94%" />
</div>

<sub>근거를 누르면 그 문서 그 위치로 갑니다. "몇 쪽에 있다"가 아니라 **그 조항 위에 직접** 표시하므로,
맞는지 눈으로 바로 확인됩니다 — 위 그림에서 상자 바로 아래에 **제79조(징계의 종류)** 원문이 보입니다.</sub>

표현이 달라도 찾아냅니다. "연구윤리 위반"이라고만 물어도 그 낱말이 없는 조문까지 걸립니다.
반대로 "제7조의2"처럼 **표기가 정확히 맞아야 하는 것**도 놓치지 않습니다.

### 📚 지식베이스

규정집·논문·교재를 넣으면 찾을 수 있는 형태로 정리해 둡니다.
**PC의 폴더를 지정**하면 하위까지 자동 등록되고, PDF·HWP·워드·엑셀·PPT·전자책·스캔본을 다룹니다.

여러 개를 따로 둘 수 있습니다. 규정집과 논문, 교재를 나눠 두고 필요한 것만 골라 물어보면 됩니다.

<div align="center">
  <img src="assets/kb-sidebar.png" alt="왼쪽 지식베이스 패널 — 요약과 함께 문서 15편이 모두 적재 완료로 표시된다" width="46%" />
</div>

**분야별 스타터 지식베이스**를 준비하고 있습니다 — 법률·과학기술·경제·행정·교육.

> [!TIP]
> **법률 분야 「국가 제도·법령 (표본 15편)」은 설치본에 이미 들어 있습니다.**
> 설치하면 그 자리에서 바로 물어볼 수 있습니다.

<details>
<summary><b>무엇이 들었나</b> — 법제처 국가법령정보센터 법령 원문 15편</summary>

<br/>

| | 법령 |
| --- | --- |
| 기본 | 대한민국헌법 |
| 행정·공무원 | 국가공무원법 · 지방자치법 · 행정절차법 |
| 개인·생활 | 개인정보 보호법 · 국민건강보험법 · 주택법 |
| 국토·환경·안전 | 국토의 계획 및 이용에 관한 법률 · 환경영향평가법 · 재난 및 안전관리 기본법 |
| 공정거래·산업 | 독점규제 및 공정거래에 관한 법률 · 하도급거래 공정화에 관한 법률 · 산업집적활성화 및 공장설립에 관한 법률 |
| 연구개발 | 국가연구개발혁신법 · 국가연구개발혁신법 시행령 |

대한민국 법령은 저작권법 제7조 제1호에 따른 **비보호저작물**이라 조건 없이 재배포할 수 있습니다.

과학기술 · 경제 · 행정공공 · 교육 분야는 재배포 조건이 확정되는 대로 추가됩니다.

</details>

### 🤖 분야가 다른 다섯 에이전트

에이전트마다 **대화와 기억이 분리**되어 있습니다.
행정 업무는 하루와, 학습은 토토와 각각 이어서 진행할 수 있습니다.

| 에이전트 | 역할 | 잘하는 일 |
| --- | --- | --- |
| ✨ **별이** | 기본 비서 | 요약, 번역, 분석, 문서 전반의 질의응답 |
| 🐨 **하루** | 행정 도우미 | 공문 초안 작성, 규정·지침에서 근거 찾기 |
| 🦊 **미로** | 일 파트너 | 핵심 정리, 할 일 정리, 문서 검토 |
| 🐥 **토토** | 공부 친구 | 퀴즈 풀기, 쉬운 설명, 실력 진단 |
| 🦉 **초코** | 수업 도우미 | 문제 출제, 수업 자료 만들기 |

### 📦 파일 하나로 주고받기

지식베이스는 `.durukb`, 에이전트는 `.duruagent` 파일로 저장해 건넵니다.
받는 쪽은 **가져오기만 하면** 그대로 씁니다.

준비 작업이 무겁기 때문에 이 점이 중요합니다.
규정집 수백 권을 정리하려면 좋은 PC에서도 시간이 걸리는데,
구성원 100명이 각자 반복할 이유는 없습니다.
**담당자가 한 번 만들어 나눠 주면** 나머지는 기다림 없이 바로 검색합니다.
실제로 규정 문서 159권 분량을 옮겨 봤을 때, **다시 만드는 과정 없이 곧바로** 검색됐습니다.

나눠 줄 때는 보호 장치를 겁니다.

- **암호화** — 암호를 건 파일은 암호를 아는 사람만 엽니다. 메일이나 USB로 오가도 내용이 보이지 않습니다.
- **권한** — 읽기 전용으로 주면 받은 쪽은 보고 검색만 할 수 있고, 문서를 더 넣거나 바꿀 수는 없습니다.
- **무결성 확인** — 전송 중 파일이 손상됐는지 열기 전에 알아냅니다.

### 🔒 내 PC에서 실행

DURU는 클라우드 서비스가 아니라 **내 PC에 설치하는 프로그램**입니다.
문서도, 지식베이스도, 대화 기록도 전부 PC 안에 있습니다.
**밖에 올릴 수 없는 자료**를 다루는 자리가 DURU의 자리입니다.

AI 모델도 밖에 두지 않습니다. **Ollama**로 PC에 설치할 수 있는 소형 모델을 쓰며,
국내 독자 파운데이션 모델 **Solar**(업스테이지)·**EXAONE**(LG AI연구원) 연동을 확인했습니다.
전용 그래픽카드가 없어도 동작하고, **인터넷이 끊긴 내부망에서도** 씁니다.

> [!TIP]
> **서버에 두고 조직이 함께 쓰는 구성이 필요하다면 [DOREA-X](https://github.com/leeryong/DOREA-X)** 를 보십시오.
> 같은 계열의 서버형 제품입니다. 자료를 서버에 올릴 수 있고 운영을 맡을 조직이 있다면 그쪽이 맞고,
> 그렇지 않다면 DURU가 맞습니다 — [어디에 무엇이 맞는지](docs/DURU.md#-6-로컬-실행--자료-보호)

---

## 📖 더 자세히

지식베이스가 무엇인지, 다섯 에이전트가 어떻게 구성되는지,
근거를 어떻게 제시하는지, 패키지로 어떻게 주고받는지

→ **[DURU 소개](docs/DURU.md)**

---

## 📥 배포

| | |
| --- | --- |
| **DURU Setup 0.8.0.exe** | 윈도우 10/11 (64비트) · 약 300MB · [내려받기](../../releases/latest) |

설치본 안에 **지식베이스 「국가 제도·법령 (표본 15편)」이 들어 있습니다.** 첫 실행 때 한 번
자동으로 준비되므로 따로 받거나 가져올 필요가 없습니다.
남에게 건네거나 다시 넣고 싶을 때만 `.durukb` 파일을 따로 받으면 됩니다.

| 따로 받고 싶다면 | |
| --- | --- |
| **국가 제도·법령 (표본 15편).durukb** | 약 70MB · [내려받기](../../releases/latest) |

> [!NOTE]
> 🍎 **맥(macOS)판은 곧 공개합니다.** 지금은 윈도우판만 있습니다.
> 준비되는 대로 이 페이지와 [Releases](../../releases) 에 올리겠습니다.
> 쓰는 방법은 윈도우와 같고, 설치 파일(`.dmg`)을 열어 DURU 를 `응용 프로그램` 폴더로
> 끌어다 놓는 것만 다릅니다.

**설치**

1. 내려받은 `.exe`를 실행합니다. 코드서명이 없어 처음에 SmartScreen 경고가 뜹니다 → **추가 정보 → 실행**.
2. 처음 켜면 상단 배너가 **문서 파서** 받기를 안내합니다. 한 번만 받으면 됩니다(약 1.1GB).
3. 답할 모델을 고릅니다 — 설정 → 대화창 → LLM. 내 그래픽카드를 보고 알맞은 것을 권해 줍니다.

<div align="center">
  <img src="assets/settings-llm.png" alt="설정 → 대화창 → LLM. 설치된 모델과 추천 모델이 보인다" width="88%" />
</div>

4. 지식베이스 `.durukb` 파일을 화면에 끌어다 놓거나, 설정 → 지식베이스 → **가져오기**.

**처음이라면** — 가운데 화면에 세 걸음 안내가 뜹니다. 그대로 따라 하면 됩니다.
앱 안에서 오른쪽 위 책 아이콘을 누르면 **사용설명서**(14편)가 열립니다.

<div align="center">
  <img src="assets/manual-in-app.png" alt="앱 안에서 바로 열리는 사용설명서" width="88%" />
</div>

---

## 🌌 관련 프로젝트

DURU는 KISTI **BLUESKY** 프로젝트의 문서 AI 기술 위에서 만들어졌습니다.

| 시스템 | 소개 |
| --- | --- |
| 🌌 [KISTI-NTIS BLUESKY](https://github.com/leeryong/KISTI_BLUESKY) | 사람과 AI의 협업을 향한 프로젝트 허브 |
| 📄 [DOREA-X](https://github.com/leeryong/DOREA-X) | **서버형** — 조직이 함께 쓰는 문서 AI. 문서 이해·분석·보고서 작성 |
| 🛠️ [NELLA](https://github.com/leeryong/NELLA) | 문서로 도메인 특화 LLM을 만드는 Agentic LLMOps |
| 🎩 [Scarlet](https://github.com/leeryong/Scarlet) | 멀티에이전트 지식 탐색·추론 (홈즈–왓슨) |
| 🌐 [TAW (The Agents Web)](https://github.com/leeryong/The_Agents_Web_TAW/blob/main/README.ko.md) | 에이전트와 사람이 함께 일하는 에이전트 웹 |
| 🗂️ [ParserTry](https://github.com/leeryong/ParserTry) | 30종 PDF 파서 즉시 실행·비교 로컬 웹앱 |

---

## 📄 기대어 만든 공개 소스

DURU는 아래 공개 소스 위에서 동작합니다. 라이선스가 표시를 요구하는 것들입니다.

| 하는 일 | 쓰는 것 |
| --- | --- |
| 문서 읽기 | [OpenDataLoader PDF](https://github.com/opendataloader-project/opendataloader-pdf) `Apache-2.0` · [Docling](https://github.com/docling-project/docling) `MIT` · [pypdfium2 / PDFium](https://github.com/pypdfium2-team/pypdfium2) `Apache-2.0, BSD-3` · [pdfplumber](https://github.com/jsvine/pdfplumber) `MIT` · [MarkItDown](https://github.com/microsoft/markitdown) `MIT` · [pikepdf](https://github.com/pikepdf/pikepdf) `MPL-2.0` |
| 글자 인식(OCR) | [PaddleOCR](https://github.com/PaddlePaddle/PaddleOCR) `Apache-2.0` · [Tesseract](https://github.com/tesseract-ocr/tesseract) `Apache-2.0` · [manga-ocr](https://github.com/kha-white/manga-ocr) `Apache-2.0` |
| 찾기·기억 | [Qdrant](https://github.com/qdrant/qdrant) `Apache-2.0` · [Mem0](https://github.com/mem0ai/mem0) `Apache-2.0` · [BGE-M3](https://huggingface.co/BAAI/bge-m3) `MIT` |
| AI 모델 실행 | [Ollama](https://github.com/ollama/ollama) `MIT` · [PyTorch](https://github.com/pytorch/pytorch) `BSD-3` · [ONNX Runtime](https://github.com/microsoft/onnxruntime) `MIT` |
| 프로그램 뼈대 | [FastAPI](https://github.com/fastapi/fastapi) `MIT` · [Uvicorn](https://github.com/encode/uvicorn) `BSD-3` · [SQLAlchemy](https://github.com/sqlalchemy/sqlalchemy) `MIT` · [Pydantic](https://github.com/pydantic/pydantic) `MIT` · [SQLite](https://www.sqlite.org/) `퍼블릭 도메인` |
| 화면 | [React](https://github.com/facebook/react) `MIT` · [Vite](https://github.com/vitejs/vite) `MIT` · [PDF.js](https://github.com/mozilla/pdf.js) `Apache-2.0` · [Tailwind CSS](https://github.com/tailwindlabs/tailwindcss) `MIT` · [Radix UI](https://github.com/radix-ui/primitives) `MIT` · [Pillow](https://github.com/python-pillow/Pillow) `MIT-CMU` |
| 도구 연결 | [Model Context Protocol](https://github.com/modelcontextprotocol) `MIT` |

> [!NOTE]
> 만화·잡지 번역에 쓰는 **[comic-translate](https://github.com/ogkalu2/comic-translate)** `GPL-3.0` 은
> 설치본에 담기지 않습니다. 사용자가 따로 띄운 프로그램과 **HTTP로 통신할 뿐**입니다.

**전체 목록은 앱 안에 있습니다** — 설정 → 시스템 → 정보. 각 항목의 역할·라이선스·주소를 함께 밝힙니다.

## 🙏 부탁드립니다

**많이 써 보시고, 느낀 점을 알려 주십시오.**

DURU는 쓰는 사람의 자리에서 만들어졌습니다. 어떤 문서를 넣었는데 잘 안 읽히더라,
이런 걸 물었는데 엉뚱한 걸 가져오더라, 이 화면은 무슨 뜻인지 모르겠더라 —
그런 이야기가 다음 판을 만듭니다.

- 🐞 **잘 안 되는 것** — 어떤 문서로 무엇을 하려다 어떻게 됐는지 적어 주시면 재현해 봅니다
- 💡 **있었으면 하는 것** — 업무에서 실제로 막히는 자리를 알려 주십시오
- 📚 **지식베이스** — **분야별 지식베이스가 필요하시면 연락 주십시오.**
  지금은 법률 분야만 공개돼 있습니다. 과학기술 · 경제 · 행정공공 · 교육 등 필요한 분야를
  알려 주시면 우선순위를 정해 만들겠습니다. 기관 자료로 만들어 쓰는 방법도 안내해 드립니다.
- 🍎 **맥용이 필요하시면** 알려 주십시오 — 준비되는 대로 이 페이지에서 알려 드리겠습니다.

---

## 👨‍💻 개발자 그룹

KISTI **BLUESKY** 팀 — *Harmonizing Human and AI Collaboration* · [github.com/leeryong/KISTI_BLUESKY](https://github.com/leeryong/KISTI_BLUESKY)

* 이용 ([ryonglee@kisti.re.kr](mailto:ryonglee@kisti.re.kr))

---

## 📞 문의

* 이용 ([ryonglee@kisti.re.kr](mailto:ryonglee@kisti.re.kr))

---

<div align="center">
  <sub>
    <b>DURU</b> · 두루 돕는 AI — KISTI BLUESKY
  </sub>
</div>
