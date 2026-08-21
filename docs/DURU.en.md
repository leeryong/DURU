# 📚 DURU — AI That Helps All Around

<div align="right">

[한국어](DURU.md) | **English**

</div>

> Register documents, ask questions, check the sources.
> This page follows the [overview](../README.en.md#-at-a-glance) in the README and goes into how it works.

---

## 🤔 The situation

A hundred and sixty rulebooks sit in a folder. Your manager asks:

> "That business trip — can it be reimbursed without a hotel receipt?"

You press `Ctrl+F` and search for "lodging". Eighty-four hits. Which rulebook, which article,
whether an exception applies, whether it was amended last year… in the end you phone someone who knows.

Ask a general chatbot and you get a confident-sounding answer. The problem is that it has no idea
whether that reflects *your* organization's rules. It may even invent an article that does not exist.
Where rules are concerned, that is not help — it is a hazard.

DURU looks only inside the documents you registered, and tells you which document and which page.

---

## 📦 1. Knowledge base — the foundation

### In short

> Your pile of documents, organized so an AI can actually read it.

Putting books on a shelf is one thing; having read them all and knowing where each topic lives
is another. A knowledge base is the second one.

### ⚙️ How a document is processed

Drop in a PDF and DURU does this.

| Step | What happens |
|---|---|
| **Read** | Reads each page — including *where* the text, tables, and figures sit |
| **Organize** | Splits it into coherent units and prepares them so they can be found later |
| **Store** | Keeps it in a searchable form |

Once that is done, your documents are not re-read on every question.

### 🔍 How it searches — by meaning and by exact wording

Ask about "research misconduct" and DURU will surface pages where that phrase never appears —
because *"malpractice"*, *"integrity review"*, and *"disciplinary measures"* are connected in meaning.

Conversely, something like "Article 7-2", where the exact form must match, is not missed either.
Article numbers, proper nouns, and technical terms fall into this category.

DURU looks at both. Searching by meaning alone loses exact references;
searching by wording alone loses passages phrased differently. Small typos are tolerated.

> Search behaviour keeps improving as document types and question patterns are studied.

### 📊 In practice — an institutional rulebook set

Measured on one research institute's internal rulebooks.

| | |
|---|---|
| Documents | **159** (travel expenses, records, governance, research ethics, security, audit …) |
| Pages | **2,267** |
| Characters | **2,864,248** |

Reading all of it would take a person weeks. DURU organizes it once,
then pulls out only the few passages each question needs.

> You can keep several knowledge bases. Rules, papers, textbooks, and project plans can live
> separately — ask only the one you need. They do not blend together.

---

## 🤖 2. Agents — who handles the documents

If a knowledge base is the material, an agent is the person working with it.

DURU comes with five, each in a different role. They have different faces, different tones,
and separate memories.

| | Name | Role | When to call on them |
|---|---|---|---|
| ✨ | **Byeoli** | General assistant across documents | Summaries, translation, analysis — "what is this document about?" |
| 🐨 | **Haru** | Administration, finding grounds in rules | Drafting official letters — "is this permitted under our rules?" |
| 🦊 | **Miro** | Partner for organizing work | Meeting notes, action items, document review |
| 🐥 | **Toto** | Tutor for studying | Working through quizzes, plain-language explanations |
| 🦉 | **Choco** | Assistant for teaching | Writing exam questions, preparing worksheets |

### 🧩 What an agent is made of

The difference is not just appearance. Inside, an agent is:

```
Agent  =  persona  +  skills  +  knowledge base  +  model (LLM)  +  memory
```

**Persona** — written the way you would introduce a person.

| Field | Meaning | Example (rules assistant) |
|---|---|---|
| Identity | Who it is | "A specialist in this institution's internal rules" |
| Role | What it helps with | "Finds which rule applies and explains the clause and procedure" |
| Tone | How it speaks | "Precise and formal, as befits official documents" |
| Instructions | What it must always do | "Always cite the rulebook name and the article, paragraph, and item" |
| Boundaries | What it must not do | "Never guess or assert anything not in the rulebooks" |
| Policy | What to do without grounds | "Say so plainly and point to the responsible department" |

**Skills** — the things it can do. Concrete abilities can be attached, such as
"lay out rule clauses in a table" or "trace how one rule delegates to another".

**Pre-loaded memory** — background the agent should already know in its field, planted as memory.
Whoever receives it starts from that knowledge.
(Personal conversation memory that accumulates as *you* use it never travels — see section 5.)

**A dedicated model (optional)** — a small model trained to be at home with your documents'
vocabulary and phrasing can be attached.

---

## 💬 3. How answers arrive — with their sources

> "What measures apply to a research ethics violation? Include the relevant clauses."

You can watch what Byeoli is doing while the answer forms.

```
10:32:32  Processing the message…
10:32:32  Checking memory for related information…
10:32:33  Reading document summaries to decide where to look…
10:33:21  Found 5 relevant documents in the knowledge base.
10:34:44  Composing the answer…
```

Then this appears beneath the answer.

> `RAG` — 5 sources behind this answer; click one to jump to that spot in the document

Clicking really does jump there. A green box is drawn on the original, so you can see with your own
eyes what the AI was reading. Not "trust me" — "look here".

---

## 🖥️ 4. Working alongside the document viewer

> For a question about personal data protection, for instance, sources are listed like this.
>
> | Document | Page |
> |---|---|
> | Personal Data Protection Guideline | p.19 |
> | Personal Data Protection Guideline | p.17 |
> | Research Ethics Regulation | p.2 |
> | Commissioned Research Regulation | p.51 |
> | Joint Research Regulation | p.28 |
>
> Sorted by relevance; clicking one moves to that page.

- Reads **PDF, HWP, Word, Excel, PowerPoint, e-books, and scanned images**.
- Pick a document on the left, read it in the middle, ask on the right.
- Drag over a marked region to narrow the question — "just explain this table".
- Point it at a folder and everything underneath is registered automatically; when an original
  is deleted, the entry goes with it.

---

## 🎁 5. Sharing — handing over a package

This is where DURU differs a little.

Building a knowledge base takes real computation. Processing 159 rulebooks takes time
even on a capable machine, and there is no reason for every employee to do it on their own PC.

So DURU hands things over as a file.

| File | What it is | Typical use |
|---|---|---|
| `.durukb` | **Knowledge base** — documents, prepared and searchable | "Here's our department's rulebook knowledge base" |
| `.duruagent` | **Agent** — persona + skills + knowledge base + model + memory | "Take this agent as it is" |

There are two formats. An agent file already contains everything it needs to work,
so in practice a single file is often enough.

The recipient only has to import it. Because it arrives fully prepared,
searching works immediately — nothing is rebuilt.

> Importing a 159-document knowledge base required no rebuilding at all. There is no waiting.

### 📋 What travels and what does not

**Included** — persona, skills, knowledge base, dedicated model, and the pre-loaded memory
the author planted.

**Not included** — personal conversation memory (what accumulates as you use it stays yours),
chat history, and LLM settings or API keys (the recipient uses their own model).

### 🔧 Handover options

- **Encryption** — a file with a password opens only for those who know it. Its contents stay
  unreadable while it travels by email or on a USB stick.
- **Read-only / read-write** — given read-only, the recipient can view and search, but cannot add
  documents or pass it on further.
- **Integrity check** — damage in transit is detected before the file is opened.
- **Summary information** — you can see what is inside, and how much, without opening the whole file.

---

## 🔒 6. Running locally — protecting your material

DURU is a program installed on your own computer, not a cloud service.

- Documents, knowledge bases, and conversation history all stay on your PC.
- The model runs locally too. Through Ollama, DURU uses small models installed on the machine.
  Integration is confirmed with Korea's sovereign foundation models — Solar (Upstage) and
  EXAONE (LG AI Research) — and other open models can be chosen as well.
- It works on internal networks with no internet access.
- A commercial API can optionally be connected; only then does anything related to your question leave.

Company rulebooks, internal reports, unpublished research — material that cannot be uploaded anywhere
is precisely where DURU belongs.

### ⚖️ Server-side or local — which fits

Whether to put document AI on a server or on each person's PC depends on the environment.
It is not a question of performance, but of whether the material can be moved
and whether there is anyone to operate the system.

**Can the material be moved?**
A server-side system needs the documents uploaded before it can search. That is fine for public
material or documents already in internal systems. But personnel and complaint records containing
personal data require a legal basis and a review of processing arrangements; confidential reports and
unpublished research must clear an export review. An external cloud adds a cross-border transfer
review on top. It is not unusual for the documents whose answers are needed most to be the hardest to move.

**Is there anyone to operate it?**
Servers and GPUs have to be procured, the search engine and AI models kept running, accounts and
permissions managed, versions upgraded, and outages handled. This is not a one-off build but ongoing
work, so it needs staff and budget continuously. For an organization with dedicated people it is a
natural choice; at the level of a department or an individual, those conditions are hard to meet.

| | Server-side fits when | DURU fits when |
| --- | --- | --- |
| Material | Everyone works from **the same documents** | Documents differ per person, or cannot leave |
| Operations | Dedicated staff and budget exist | There is no one to operate it |
| Scale | Large-scale concurrent use | Individual or small teams |

DURU took the right-hand column. Nothing is uploaded, so no review is triggered; running the installer
puts it on each person's PC, so no operations team is needed. Knowledge bases that need heavy
preparation are built once by one person and handed out as files
(→ [5. Sharing](#-5-sharing--handing-over-a-package)).

> If the server-side column fits your environment, **[DOREA-X](https://github.com/leeryong/DOREA-X)**
> is the counterpart in the same family — the configuration an organization runs on a server.
> The two are not mutually exclusive; depending on the material and your operating conditions,
> they can be used separately or together.

---

## 📥 Getting started and requirements

Install → register documents → ask. Making those three steps sufficient is the design goal.
Neither knowledge bases nor agents have to be built yourself — both can arrive as files.
When someone in the organization builds them once and distributes them, everyone else just imports.

**Requirements** — an ordinary office PC is enough. A graphics card makes it faster but is not required.
Because the heavy computation is finished by whoever hands the package over,
the receiving machine can be modest.

**Availability** — Windows and macOS installers are in preparation.
This repository will carry the announcement when they are released.

---

<div align="center">
  <sub><b>DURU</b> · AI that helps all around — KISTI-NTIS BLUESKY · Contact: Ryong Lee (ryonglee@kisti.re.kr)</sub>
</div>
