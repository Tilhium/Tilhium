<!-- ═══════════════════ BOOT SEQUENCE ═══════════════════ -->
<p align="center">
  <img src="./assets/hud-banner.svg" width="100%" alt="HUD banner" />
</p>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Share+Tech+Mono&size=20&pause=900&color=00E5FF&center=true&vCenter=true&width=680&lines=%3E+Booting+personal+systems...;%3E+AI+%C2%B7+Embedded+Linux+%C2%B7+Full-Stack;%3E+Spinning+up+local+LLMs+(qwen3+%C2%B7+llama3)...;%3E+Compiling+a+custom+kernel...+done;%3E+All+systems+online.+Welcome+back." alt="boot sequence" />
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/okan-can-camc%C4%B1/"><img src="https://img.shields.io/badge/LinkedIn-0D1117?style=for-the-badge&logo=data%3Aimage%2Fsvg%2Bxml%3Bbase64%2CPHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI%2BPHJlY3Qgd2lkdGg9IjI0IiBoZWlnaHQ9IjI0IiByeD0iNCIgZmlsbD0iIzAwRTVGRiIvPjx0ZXh0IHg9IjQuNSIgeT0iMTgiIGZvbnQtZmFtaWx5PSJBcmlhbCxIZWx2ZXRpY2Esc2Fucy1zZXJpZiIgZm9udC13ZWlnaHQ9IjcwMCIgZm9udC1zaXplPSIxNSIgZmlsbD0iIzBEMTExNyI%2BaW48L3RleHQ%2BPC9zdmc%2B" /></a>
  <a href="mailto:camciokancan@gmail.com"><img src="https://img.shields.io/badge/Comms_Channel-0D1117?style=for-the-badge&logo=gmail&logoColor=00E5FF" /></a>
  <img src="https://img.shields.io/badge/Istanbul,_TR-0D1117?style=for-the-badge&logo=googlemaps&logoColor=00E5FF" />
  <img src="https://komarev.com/ghpvc/?username=Tilhium&style=for-the-badge&color=0D1117&label=VISITORS+DETECTED" />
</p>

<br/>

## `◉ SUBJECT PROFILE`

```yaml
# ───────────────────────────── IDENTITY SCAN COMPLETE ─────────────────────────────
designation     : Okan Can Çamcı
callsign        : Tilhium
class           : Computer Engineering — 4th year (Class of 2027)
training        : YÖK Digital University · AI School 2026–2027
                  (Modern Software Development & Machine Learning)
base            : Istanbul, Türkiye 🇹🇷
status          : ONLINE ●
primary_ops     : [AI & Data Science, Systems & Embedded, Full-Stack & Mobile]
specialties     : [Local LLMs, Multi-Agent Systems, Custom Linux, Computer Vision]
operating_style : "Build the whole stack — from the kernel to the dashboard."
threat_level    : "Will automate anything done twice."
```

I'm a 4th-year computer engineering student in Istanbul who likes working where **hardware, systems and AI meet**.
I build custom Linux distributions with Buildroot, write encrypted telemetry in C, run **local LLMs** with Ollama,
and wire it all together with backends, dashboards and mobile apps.
On the data side I work on **explainable ML** — XGBoost models made readable with SHAP and LLM-generated insights.

<br/>

## `◉ PRIMARY OPERATIONS`

### 🛰️ TilthOS & ZDuruOS — custom embedded Linux

> Minimal Linux systems built from scratch with **Buildroot**, running under QEMU / VirtualBox,
> with **kernel modules** and **encrypted telemetry daemons written in C**.

TilthOS powers the edge side of the **[Tilth Detection System](https://github.com/Tilhium/Tilth-Detection-Project)**,
an Edge-AI Command & Control simulation that models a UAV ↔ ground-station link:

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

### 🧠 Churn & Retention Analytics — explainable ML

> Customer churn prediction with **XGBoost**, explained feature by feature with **SHAP**,
> and turned into plain-language retention insights by a **local LLM**.

### 🤖 Distributed Multi-Agent Software Platform — team project

> An **orchestrator agent** breaks a software requirement into tasks, scores sub-agents by their measured
> capabilities and assigns the work to worker PCs running local LLMs over **Tailscale**. Built with Scrum.
> I own the project contract, requirements and setup documentation.
> **[→ repository](https://github.com/Tilhium/dap_test)**

<br/>

## `◉ MISSION LOG`

| Codename | Briefing | Tech | Status |
|---|---|---|---|
| [**Tilth Detection**](https://github.com/Tilhium/Tilth-Detection-Project) | Edge-AI C2 simulation: TilthOS, AES-256 telemetry, YOLOv8 detection, React tactical dashboard | `C` `Buildroot` `YOLOv8` `Node.js` `React` | 🟢 `DEPLOYED` |
| [**Distributed AI Platform**](https://github.com/Tilhium/dap_test) | Orchestrator + sub-agent architecture distributing software tasks to local LLM workers | `FastAPI` `SQLAlchemy` `Ollama` `React` `TS` | 🟡 `IN PROGRESS` |
| **ZDuruOS** | Second Buildroot-based minimal Linux with kernel modules and encrypted telemetry | `C` `Buildroot` `QEMU` | 🔒 `CLASSIFIED` |
| **Churn & Retention Analytics** | XGBoost churn model + SHAP explainability + local-LLM insight reports | `Python` `XGBoost` `SHAP` `Ollama` | 🔒 `CLASSIFIED` |
| **F.R.I.D.A.Y.** | Personal voice assistant | `Python` `LLM` | 🔒 `CLASSIFIED` |
| **Local File Summarizer** | Ollama agent that reads and summarizes files on the local disk | `Python` `Ollama` | 🔒 `CLASSIFIED` |
| [**Focus**](https://github.com/Tilhium/Focus_Productivity_App) | Desktop productivity app: tasks, Pomodoro stats, book & anime tracking, Notion-style wiki, semantic search with embeddings | `FastAPI` `sqlite-vec` `pywebview` | 🟢 `DEPLOYED` |
| [**Sirius Chat**](https://github.com/Tilhium/Sirius-Chat-App-Demo) | Real-time messenger with AES-encrypted messages, brute-force lockout, rooms, friends and media sharing | `React` `Socket.io` `Express` `MongoDB` | 🟢 `DEPLOYED` |
| [**Academic Journal Automaton**](https://github.com/Tilhium/Journal-Automation-Website) | Role-based manuscript life cycle: submission, reviewer assignment, PDF annotation, editorial decision | `Flask` `SQLAlchemy` `SQLite` | 🟢 `DEPLOYED` |
| **DB Architecture Tool** | Tool for designing database architectures | `SQL` `Python` | 🔒 `CLASSIFIED` |
| **Modular Encryption Suite** | Collection of modular encryption projects | `C` `Python` | 🔒 `CLASSIFIED` |
| [**Podcast Player**](https://github.com/Tilhium/PodcastPlayer-App) | Cross-platform podcast player | `Flutter` `Dart` | 🟢 `DEPLOYED` |

<sub>🔒 `CLASSIFIED` = not public yet.</sub>

<br/>

## `◉ CAPABILITY MATRIX`

| Domain | Systems |
|---|---|
| 🧠 **AI & Data Science** | Machine learning · XGBoost · SHAP · Ollama (`qwen3`, `qwen2.5`, `llama3`) · multi-agent systems · OpenCV · YOLOv8 · Jupyter |
| 🛰️ **Systems & Embedded** | Buildroot (TilthOS, ZDuruOS) · Linux kernel modules · C systems programming · ARM Cortex-M4 / STM32F407 · compiler design (Flex) |
| ⚙️ **Backend** | Python (FastAPI, Flask) · Node.js / Express · Socket.io · SQL |
| 🖥️ **Frontend & Mobile** | JavaScript · React · TypeScript · Vite · Flutter / Dart |
| 🔐 **Security** | AES-256-CBC · encrypted telemetry · bcrypt · token auth · brute-force protection |
| 🗄️ **Data** | MySQL · SQLite · sqlite-vec · MongoDB · SQLAlchemy |
| 🧰 **Environment** | Linux · WSL2 (Ubuntu) · Docker · Tailscale · QEMU · VirtualBox · Git & GitHub |

<br/>

## `◉ LOADED MODULES`

<p align="center">
  <img src="https://skillicons.dev/icons?i=c,cpp,python,js,ts,dart,java&theme=dark" /><br/>
  <img src="https://skillicons.dev/icons?i=fastapi,flask,nodejs,express,react,vite,flutter&theme=dark" /><br/>
  <img src="https://skillicons.dev/icons?i=opencv,mysql,sqlite,mongodb,linux,ubuntu,docker,git,github&theme=dark" />
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
+ YÖK Digital University AI School — modern software development & machine learning
+ Building a distributed multi-agent LLM platform with my team
+ Going deeper into kernel modules, STM32 firmware and custom Linux builds
+ Making ML models explainable with SHAP + local LLMs
! Open to internships and collaboration in AI, embedded systems or full-stack work
```

<br/>

## `◉ OFF-DUTY SUBROUTINES`

<p align="center">
  <img src="https://img.shields.io/badge/Calisthenics-0D1117?style=for-the-badge&logo=strava&logoColor=FFB300" />
  <img src="https://img.shields.io/badge/Acoustic_Guitar-0D1117?style=for-the-badge&logo=applemusic&logoColor=FFB300" />
  <img src="https://img.shields.io/badge/Vocal_Training-0D1117?style=for-the-badge&logo=audiomack&logoColor=FFB300" />
  <img src="https://img.shields.io/badge/Drawing_%26_Illustration-0D1117?style=for-the-badge&logo=krita&logoColor=FFB300" />
  <br/>
  <img src="https://img.shields.io/badge/Plant_Care-0D1117?style=for-the-badge&logo=leaflet&logoColor=FFB300" />
  <img src="https://img.shields.io/badge/Budgie_Keeper-0D1117?style=for-the-badge&logo=parrotsecurity&logoColor=FFB300" />
  <img src="https://img.shields.io/badge/Anime_%26_Manga-0D1117?style=for-the-badge&logo=myanimelist&logoColor=FFB300" />
  <img src="https://img.shields.io/badge/Gaming-0D1117?style=for-the-badge&logo=steam&logoColor=FFB300" />
</p>

<br/>

<p align="center">
  <img src="./assets/hud-footer.svg" width="100%" alt="end of transmission" />
</p>
