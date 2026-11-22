<!-- ═══════════════════ BOOT SEQUENCE ═══════════════════ -->
<p align="center">
  <img src="./assets/hud-banner.svg" width="100%" alt="HUD banner" />
</p>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Share+Tech+Mono&size=20&pause=900&color=00E5FF&center=true&vCenter=true&width=640&lines=%3E+Booting+personal+systems...;%3E+Edge+AI+%C2%B7+Embedded+Linux+%C2%B7+Full-Stack;%3E+Encrypting+telemetry+with+AES-256...;%3E+Orchestrating+multi-agent+LLMs...;%3E+All+systems+online.+Welcome+back." alt="boot sequence" />
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/okan-can-camc%C4%B1/"><img src="https://img.shields.io/badge/LinkedIn-0D1117?style=for-the-badge&logo=linkedin&logoColor=00E5FF" /></a>
  <a href="mailto:camciokancan@gmail.com"><img src="https://img.shields.io/badge/Comms_Channel-0D1117?style=for-the-badge&logo=gmail&logoColor=00E5FF" /></a>
  <img src="https://komarev.com/ghpvc/?username=Tilhium&style=for-the-badge&color=0D1117&label=VISITORS+DETECTED" />
</p>

<br/>

## `◉ SUBJECT PROFILE`

```yaml
# ───────────────────────────── IDENTITY SCAN COMPLETE ─────────────────────────────
designation     : Okan Can Camcı
callsign        : Tilhium
class           : Computer Engineering Student
base            : Türkiye 🇹🇷
status          : ONLINE ●
primary_ops     : [Edge AI, Embedded Linux, Full-Stack Web, LLM Agents]
specialties     : [Computer Vision, Secure Comms, Real-Time Systems]
side_quests     : [Compilers, Productivity Tools, Mobile Apps]
operating_style : "Build the whole stack — from the kernel to the dashboard."
threat_level    : "Will automate anything done twice."
```

I'm a computer engineering student who enjoys systems where **hardware, networking and AI meet**.
My favourite builds go end to end: a custom Linux image on the edge, encrypted data over the wire,
a model that understands it, and a live dashboard that shows it all.
Lately I've been working with **local LLMs and multi-agent systems**, and on the side I write
tools that make my own life easier: a productivity app with semantic search, lab-report generators,
and even a small compiler.

<br/>

## `◉ PRIMARY OPERATION — TILTH DETECTION SYSTEM`

> An **Edge-AI Command & Control (C2) simulation** that models a UAV ↔ ground-station link.
> A custom embedded Linux on the edge streams encrypted telemetry, a YOLOv8 vision module detects targets,
> and everything converges on a real-time tactical dashboard.

```mermaid
%%{init: {'theme':'dark', 'themeVariables': {'primaryColor':'#0D1117','primaryBorderColor':'#00E5FF','primaryTextColor':'#E6F7FF','lineColor':'#00E5FF','clusterBkg':'#07131C','clusterBorder':'#5FB8C9'}}}%%
flowchart LR
  subgraph EDGE["🛰️ EDGE NODE — TilthOS"]
    D["C daemon<br/>reads /proc/loadavg"]
  end
  subgraph GCS["🏢 GROUND CONTROL STATION"]
    V["YOLOv8 vision<br/>Python + OpenCV"]
    S["Command server<br/>Node.js + Express"]
    UI["C2 dashboard<br/>React + Vite"]
  end
  D -- "AES-256-CBC · TCP :4000" --> S
  V -- "Socket.io :3000 · token auth" --> S
  S -- "live sync" --> UI
```

- **TilthOS:** a ~250 MB minimal Linux distro built from scratch with **Buildroot**, running under **QEMU**
- **Edge daemon:** statically compiled **C** program using POSIX system calls, encrypting telemetry with **AES-256-CBC**
- **Dual-channel backend:** Node.js merges raw TCP sensor data and authenticated WebSocket AI detections in real time
- **Tactical UI:** React dashboard that shows AI detections and edge-device CPU load side by side

[`▶ OPEN MISSION FILE`](https://github.com/Tilhium/Tilth-Detection-Project)

<br/>

## `◉ MISSION LOG`

| Codename | Briefing | Tech | Status |
|---|---|---|---|
| [**Tilth Detection**](https://github.com/Tilhium/Tilth-Detection-Project) | Edge-AI C2 simulation: custom Buildroot Linux, AES-256 telemetry, YOLOv8 detection, React tactical dashboard | `C` `Python` `YOLOv8` `Node.js` `React` | 🟢 `DEPLOYED` |
| [**Distributed AI Dev Platform**](https://github.com/Tilhium/dap_test) | Team project: a master agent splits a software requirement into tasks and assigns them to worker PCs running local LLMs (Ollama). Run with Scrum over five sprints | `FastAPI` `SQLAlchemy` `Ollama` `React` `TypeScript` | 🟡 `IN PROGRESS` |
| [**Focus**](https://github.com/Tilhium/Focus_Productivity_App) | AI-powered all-in-one productivity app: tasks, Pomodoro stats, book & anime tracking (AniList GraphQL), Notion-style wiki and semantic search with embeddings. Runs on desktop and web | `FastAPI` `sqlite-vec` `pywebview` `JavaScript` | 🟢 `DEPLOYED` |
| [**Sirius Chat**](https://github.com/Tilhium/Sirius-Chat-App-Demo) | Real-time messenger with AES-encrypted messages, brute-force lockout, group rooms, friend system, media sharing and read receipts | `React` `Socket.io` `Express` `MongoDB` | 🟢 `DEPLOYED` |
| [**Academic Journal Automaton**](https://github.com/Tilhium/Journal-Automation-Website) | Role-based platform covering a manuscript's full life cycle: submission, reviewer assignment, interactive PDF annotation, editorial decision | `Flask` `SQLAlchemy` `Alembic` `SQLite` | 🟢 `DEPLOYED` |
| [**Podcast Player**](https://github.com/Tilhium/PodcastPlayer-App) | Cross-platform podcast player app | `Dart` `Flutter` | 🟢 `DEPLOYED` |
| [**Text-to-Speech Converter**](https://github.com/Tilhium/Text-to-Speech-Converter-app-PythonFlask) | Web app that turns text into speech | `Python` `Flask` | 🟢 `DEPLOYED` |
| [**Spa Management System**](https://github.com/Tilhium/Spa-Management-System) | Desktop management system for a spa business | `Java` | 🟢 `DEPLOYED` |

<br/>

## `◉ CAPABILITY MATRIX`

| Domain | Systems |
|---|---|
| 🛰️ **Embedded & Edge** | Buildroot · QEMU · C · POSIX system calls · TCP sockets |
| 🧠 **AI / ML** | YOLOv8 · OpenCV · Ollama (local LLMs) · OpenAI API · embeddings & semantic search · Jupyter |
| 🔐 **Security** | AES-256-CBC · CryptoJS · bcrypt · token auth · brute-force protection |
| ⚙️ **Backend** | FastAPI · Flask · Node.js / Express · Socket.io · REST & GraphQL clients |
| 🖥️ **Frontend** | React · TypeScript · Vite · Tailwind · Jinja2 |
| 🗄️ **Data** | SQLite · sqlite-vec · MongoDB · MySQL · SQLAlchemy · Alembic |
| 📱 **Mobile & Desktop** | Flutter / Dart · pywebview · Java |
| 🛠️ **Low-level & Tooling** | C++ · compilers (scanner & parser) · Make · Git · Scrum |

<br/>

## `◉ LOADED MODULES`

<p align="center">
  <img src="https://skillicons.dev/icons?i=c,cpp,python,java,js,ts,dart&theme=dark" /><br/>
  <img src="https://skillicons.dev/icons?i=react,vite,tailwind,nodejs,express,fastapi,flask&theme=dark" /><br/>
  <img src="https://skillicons.dev/icons?i=flutter,opencv,mongodb,sqlite,mysql,linux,git,github&theme=dark" />
</p>

<br/>

## `◉ SYSTEM DIAGNOSTICS`

<p align="center">
  <img height="170" src="https://github-readme-stats.vercel.app/api?username=Tilhium&show_icons=true&hide_border=true&count_private=true&bg_color=0D1117&title_color=00E5FF&icon_color=FFB300&text_color=C9D1D9&ring_color=00E5FF&custom_title=SYSTEM%20DIAGNOSTICS" />
  <img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Tilhium&layout=compact&hide_border=true&langs_count=8&bg_color=0D1117&title_color=00E5FF&text_color=C9D1D9&custom_title=CORE%20LANGUAGES" />
</p>

<p align="center">
  <img src="https://streak-stats.demolab.com?user=Tilhium&hide_border=true&background=0D1117&ring=00E5FF&fire=FFB300&currStreakNum=FFFFFF&sideNums=FFFFFF&currStreakLabel=00E5FF&sideLabels=00E5FF&dates=5FB8C9&stroke=00E5FF" />
</p>

<p align="center">
  <img width="95%" src="https://github-readme-activity-graph.vercel.app/graph?username=Tilhium&bg_color=0D1117&color=5FB8C9&line=00E5FF&point=FFB300&area=true&area_color=00E5FF&hide_border=true&custom_title=POWER%20OUTPUT%20%E2%80%94%20CONTRIBUTIONS" />
</p>

<br/>

## `◉ CURRENT DIRECTIVES`

```diff
+ Building a distributed multi-agent LLM platform with my team
+ Writing a hand-made scanner & parser for a small calculator language
+ Going deeper into embedded Linux and edge computing
! Open to internships and collaboration in Edge AI, embedded or full-stack work
```

<br/>

<p align="center">
  <img src="./assets/hud-footer.svg" width="100%" alt="end of transmission" />
</p>
