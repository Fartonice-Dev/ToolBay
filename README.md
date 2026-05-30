# 🛠️ TOOLBAY

**The control panel for AI work engines**

![Status](https://img.shields.io/badge/status-active%20development-orange?style=for-the-badge)
![Ollama](https://img.shields.io/badge/Ollama-supported-success?style=for-the-badge)
![Claude Code](https://img.shields.io/badge/Claude%20Code-bridged-D97757?style=for-the-badge)
![MCP](https://img.shields.io/badge/MCP-connected-blue?style=for-the-badge)
![Built Solo](https://img.shields.io/badge/built-solo%20in%20public-blue?style=for-the-badge)
![Human + AI](https://img.shields.io/badge/Made%20by-Human%20%2B%20AI-purple?style=for-the-badge)

*One dashboard. Multiple AI brains. Safer control.* 🧠⚡

---

## ⚡ What is TOOLBAY?

TOOLBAY is **not another AI model**.

TOOLBAY is a **control dashboard for AI work engines** — a local command center for managing Claude Code, local AI through Ollama, MCP tools, memory services, diagnostics, usage tracking, and project workflow.

Think of it like the dashboard of a custom-built machine:

* The AI models are the engines.
* TOOLBAY is the control panel.
* MCP tools and plugins are the tool rack.
* Memory is the work log.
* Diagnostics show what is running.
* Pack workflows help break big projects into safer steps.

---

## 🧠 Why TOOLBAY Exists

Most AI tools work like separate boxes.

TOOLBAY is being built to bring those boxes together into one workbench so a builder does not have to jump between disconnected browser tabs, terminal windows, local servers, logs, and AI tools.

TOOLBAY is designed for:

* solo developers
* AI builders
* tinkerers
* Claude Code users
* local AI / Ollama users
* people building custom AI workflows
* people who want better control over token usage
* people who want guided troubleshooting instead of guessing

---

## ✅ Current Working State

TOOLBAY is in active development, but several core systems now work end-to-end.

### Shipped / Verified

* ✅ **ToolBay Control Panel v2**
* ✅ **Service cards** for Memory, LiteLLM, MCP Inspector, Ollama, and Dashboard
* ✅ **Start Stack** button that launches the helper stack
* ✅ **Memory Dashboard / MCP Memory service** on port `8000`
* ✅ **LiteLLM Router** on port `4000`
* ✅ **Ollama local AI path** on port `11434`
* ✅ **MCP Inspector** on ports `6274 / 6277`
* ✅ **Dashboard server** on port `3000`
* ✅ **Claude usage tracker**
* ✅ **Top-bar Claude usage widget**
* ✅ **Diagnostic Snapshot button**
* ✅ **Copy / Clear Script Output buttons**
* ✅ **Safe Repomix pack builder**
* ✅ **AgentShield safe scan launcher**
* ✅ **Health Check button**
* ✅ **MCP Inspector connection to Memory MCP**
* ✅ **Path containment security fix for `/api/preview`**
* ✅ **Deep sandbox audit reports generated**

---

## 🧪 Latest Milestone

TOOLBAY can now help build TOOLBAY.

Recent work added:

* Real stack start/check controls
* Service status cards
* Better MCP Inspector detection
* Diagnostic snapshot reports
* Claude usage/cost visibility
* Safe local checks before using Claude Code
* Deep system audit reports
* A security guard preventing `/api/preview` from reading outside the project root

This is a major workflow improvement because local checks now handle more of the boring verification work before Claude Code is used.

---

## 💸 Token Usage Control

One of TOOLBAY’s biggest goals is reducing wasted Claude Code usage.

Current workflow improvement:

1. Run local health checks first.
2. Build safe Repomix packs only when needed.
3. Use focused Claude Code handoff files.
4. Track usage with `ccusage`.
5. Show current Claude usage in the dashboard.
6. Avoid broad blind scans unless intentionally approved.

This has already reduced wasted token burn compared to earlier workflows where Claude Code could burn through usage quickly.

---

## 🧭 Simple Overview

```text
USER / BUILDER
      │
      ▼
TOOLBAY DASHBOARD
AI Work Engine Control Panel
      │
      ├── Dashboard
      ├── ToolBay Control
      ├── Guided Builder / Pack Orchestrator
      ├── Claude Code Bridge
      ├── Local Ollama Control
      ├── Memory / MCP Service
      ├── LiteLLM Router
      ├── MCP Inspector
      ├── Diagnostics
      └── Settings / Routing / Status
      │
      ▼
LOCAL TOOL STACK
      │
      ├── Claude Code
      ├── Ollama
      ├── Memory Service
      ├── LiteLLM
      ├── MCP Inspector
      ├── Repomix
      ├── AgentShield
      └── ccusage
```

---

## 🔌 Current Local Services

| Service                       |    Port | Current Status |
| ----------------------------- | ------: | -------------- |
| ToolBay Dashboard             |  `3000` | Working        |
| Memory Dashboard / MCP Memory |  `8000` | Working        |
| LiteLLM Router                |  `4000` | Working        |
| Ollama                        | `11434` | Working        |
| MCP Inspector UI              |  `6274` | Working        |
| MCP Inspector Proxy           |  `6277` | Working        |

---

## 🛠️ ToolBay Control Panel v2

The ToolBay Control panel is the main local control area.

Current controls include:

* Start Stack
* Stop Stack
* Health Check
* Check Claude Usage
* Build Safe Repomix Pack
* Run Safe AgentShield Scan
* MCP Inspector toggle
* Open Memory Dashboard
* Open LiteLLM Router
* Open MCP Inspector
* Refresh Status
* Create Diagnostic Snapshot
* Copy Script Output
* Clear Script Output

The goal is simple:

```text
Show what is running.
Start what is missing.
Check health.
Save reports.
Do not run dangerous commands blindly.
```

---

## 📊 Diagnostic Snapshot

TOOLBAY can now create a diagnostic report showing:

* current service status
* running ports
* Claude usage summary
* key file existence
* Node.js version
* platform
* dashboard root

Reports are saved under:

```text
C:\sandbox\UE-Dashboard_DIAGNOSTICS
```

This is the beginning of a future self-repair / support-bundle system.

---

## 📚 Deep Audit Reports

A deep sandbox audit generated system maps and planning files under:

```text
C:\sandbox\UE-Dashboard_AUDITS
```

Reports include:

* `TOOLBAY_SANDBOX_FILE_MAP.md`
* `TOOLBAY_SYSTEM_MAP.md`
* `TOOLBAY_HOOK_AGENT_PLUGIN_AUDIT.md`
* `TOOLBAY_UE_PLUGIN_BRIDGE_MAP.md`
* `TOOLBAY_TROUBLESHOOTING_PLAYBOOK.md`
* `TOOLBAY_NEXT_BUILD_PLAN.md`
* `TOOLBAY_RISK_REGISTER.md`
* `TOOLBAY_ENDPOINTS_AND_BUTTONS_TABLE.md`
* `TOOLBAY_FUTURE_FEATURE_CROSSWALK.md`

These reports help guide future development instead of guessing where things are wired.

---

## 🔒 Safety Notes

TOOLBAY is being built with safety gates because it controls local tools.

Current safety direction:

* no arbitrary shell execution from the browser
* allowlisted scripts only
* backups before patches
* diagnostic reports before larger changes
* restore/checkpoint planning
* no public remote access without authentication
* no open public ports
* security fixes before expansion

Recent security fix:

```text
/api/preview now blocks paths outside C:\sandbox\UE-Dashboard
```

---

## 📦 Guided Builder / Pack Orchestrator

The Pack Orchestrator is planned to evolve into a friendlier **Guided Builder**.

User-facing name idea:

```text
Guided Builder
small sublabel: Pack Orchestrator
```

Goal:

```text
Describe an idea → ask questions → make a build plan → break into safe packs → build one step at a time → test → checkpoint → continue
```

Future features:

* Workflow Mode ON/OFF
* Small Safe Packs
* Medium Packs
* Large Batch Mode
* Break Into Smaller Tasks button
* Pack dependencies
* Pass/fail gates
* Restore points
* Claude Code handoff generation
* Previous-pack regression checks

This is meant to make TOOLBAY useful for everyday people building websites, apps, mods, dashboards, tools, or AI projects.

---

## 🗂️ Project Workspace

Planned future feature:

```text
Project Workspace
small sublabel: Scope + Context Map
```

This area will define where TOOLBAY is allowed to work.

Examples:

* one folder only
* multiple folders
* multi-service project
* editable folders
* reference-only folders
* protected folders
* ignored folders

The goal is to keep AI workers from drifting off-track.

---

## 🖼️ Reference Vault

Planned future feature:

```text
Reference Vault
small sublabel: Project References / Context Assets
```

Users should be able to attach:

* screenshots
* UI mockups
* photos
* diagrams
* code snippets
* logs
* text documents
* design notes
* URLs
* example files

Each reference should have:

* title
* type
* description
* tags
* source
* date added
* permission mode

Permission modes:

* Reference-only
* Editable copy
* Protected
* Ignore

This gives the AI the same kind of reference context a human builder would use.

---

## 🧠 Future AI Idea Helper

A future local Ollama-powered helper may act like an idea interviewer.

It should help users:

1. explain what they want to build
2. answer guided questions
3. define the interface
4. define inputs and outputs
5. define the end goal
6. define constraints
7. turn the idea into a master plan
8. break it into build packs

This is meant to help normal users turn rough ideas into working projects.

---

## 🔊 Accessibility Direction

TOOLBAY should become friendly for users with reading, memory, or attention difficulties.

Planned voice/accessibility controls:

* text-to-speech
* speech-to-text
* play
* pause
* stop
* skip forward
* skip back
* replay
* read selected section
* copy text
* save report

Areas that should support reading aloud:

* Dashboard chat
* Guided Builder
* Script Output
* Diagnostic Snapshot
* Troubleshooting reports
* Setup wizard
* Pack files
* Error output

---

## 📱 Remote / Mobile Direction

Remote control is planned later, but only after local controls are safe.

Possible future direction:

* phone-friendly dashboard
* secure login
* device pairing
* approval prompts
* read-only mode by default
* emergency stop
* encrypted tunnel or VPN
* no open public ports
* no arbitrary shell execution

Reference projects to study later:

* Claude Code Remote Control docs
* RemoteCC
* Claude-Code-Remote
* 247 Claude Code Remote
* Claude Remote Terminal
* Happy

---

## 🧩 MCP / Plugins / Agents

TOOLBAY is being built around MCP and plugin-friendly workflows.

Current MCP/tooling stack includes references to:

* GitNexus
* Memory Service
* ECC Context7
* ECC Exa
* ECC GitHub
* ECC Memory
* ECC Playwright
* ECC Sequential Thinking
* Oh My Claude Code
* Serena
* Graphify
* Repomix
* AgentShield
* ccusage

Important note:

Some hook/skill/agent/plugin counts are still estimates or UI-display values. Future work will make those counts live and verifiable.

---

## 🚧 Known Placeholder Areas

Some areas exist visually but still need backend wiring.

Known placeholders / future work:

* Brain Routing
* Break Into Packs
* Pack test runner
* Rollback restore flow
* Work Console
* Project Workspace
* Reference Vault
* Mobile Remote
* Installer / self-repair wizard
* Live hook/skill/agent counts
* LiteLLM as a routed chat provider

---

## 🧱 Coming Next

Recommended near-term build order:

1. Live-test `/api/preview` after the security guard fix
2. Add proper project workspace/scope selection
3. Improve Guided Builder / Pack Orchestrator wording
4. Wire Break Into Packs backend
5. Add pack files and pass/fail state
6. Add restore/checkpoint handling
7. Add Work Console / process output split
8. Wire LiteLLM as a second chat provider
9. Improve Brain Routing truth/status
10. Add screenshot/reference vault planning

---

## 📸 Screenshots

Current screenshots should live here:

```text
docs/screenshots/current/
```

Recommended current screenshot names:

```text
docs/screenshots/current/dashboard.png
docs/screenshots/current/toolbay-control-v2.png
docs/screenshots/current/diagnostic-snapshot.png
docs/screenshots/current/mcp-inspector-connected.png
docs/screenshots/current/settings-test-all.png
docs/screenshots/current/guided-builder-pack-orchestrator.png
docs/screenshots/current/skills-agents.png
```

### Dashboard

![TOOLBAY Dashboard](docs/screenshots/current/dashboard.png)

### ToolBay Control Panel v2

![TOOLBAY Control Panel v2](docs/screenshots/current/toolbay-control-v2.png)

### Diagnostic Snapshot

![TOOLBAY Diagnostic Snapshot](docs/screenshots/current/diagnostic-snapshot.png)

### MCP Inspector Connected

![TOOLBAY MCP Inspector Connected](docs/screenshots/current/mcp-inspector-connected.png)

### Settings / Test All

![TOOLBAY Settings Test All](docs/screenshots/current/settings-test-all.png)

### Guided Builder / Pack Orchestrator

![TOOLBAY Guided Builder Pack Orchestrator](docs/screenshots/current/guided-builder-pack-orchestrator.png)

### Skills & Agents

![TOOLBAY Skills and Agents](docs/screenshots/current/skills-agents.png)

---

## 🗃️ Screenshot Archive Plan

Old screenshots should be saved instead of deleted.

Recommended structure:

```text
docs/screenshots/archive/stage-01-dashboard-foundation/
docs/screenshots/archive/stage-02-claude-bridge/
docs/screenshots/archive/stage-03-toolbay-control-v2/
docs/screenshots/archive/stage-04-diagnostics-and-audit/
```

Each time the UI changes for the night:

1. move older screenshots into the matching archive stage
2. upload new screenshots into `docs/screenshots/current/`
3. update this README if names changed
4. commit with a short update message

---

## 🚀 Long-Term Goal

The long-term goal is a full AI workbench where:

* local AI
* cloud AI
* memory
* MCP tools
* diagnostics
* safety gates
* project packs
* guided building
* screenshots/references
* testing
* restore points
* project automation

can all work together from one control panel.

---

## 🧱 Built By

Built solo, in public, by a hands-on builder learning and shipping one piece at a time.

**#AI #LocalAI #DevTools #ClaudeCode #Ollama #MCP #BuildInPublic #IndieBuilder**

---

© 2026 · TOOLBAY is a personal project in active development · All rights reserved
