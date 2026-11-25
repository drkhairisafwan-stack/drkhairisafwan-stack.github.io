# Hermes Passover File — Setup Template

**Purpose:** Template for Dr Khairi to hand over to his USM friend (or anyone) so they can set up their own Hermes, understand what was installed, and why.

**Status:** TEMPLATE — fill in bracketed fields before handing over.

---

## 1. What has been done (summary)

- Hermes desktop agent installed and logged in on [machine name / user account]
- Claude models connected: Haiku (fast), Sonnet (standard), Opus (deep)
- Second-opinion model configured: GPT-6 Luna (via OpenCode Go)
- Specialist bots active: [list: e.g. cremabot, drphbot, vision, friday, llmbot, edith, cremascout, dummy, ultron]
- Local LLM (Ollama) set up on Mac for private/offline use: [yes / no]
- GitHub Pages site deployed: [URL or "pending"]
- Guardrails enabled: no auto-post, no paid spend without OK, archive not delete

**Date set up:** [date]  
**Set up by:** Dr Mohd Khairi Safwan bin Johari  
**Handed over to:** [name]

---

## 2. Skills installed (Hermes agent)

| Skill | What it does | Reason installed |
|-------|-------------|------------------|
| teach-ai-layman | Teach AI to non-technical people with analogies and drills | So the user can teach AI to others (e.g. USM friend) |
| teach | Agent teaches the user a skill via lesson workspace | General teaching framework |
| learning-loop | Weekly agent self-improvement from log corrections | Keeps Hermes improving automatically |
| web-design-guidelines | Reviews UI code against interface guidelines | Quality check on web deliverables |
| animated-html-deck | Builds animated slide decks (offline HTML) | Presentations and reports |
| [add more as installed] | | |

*(Full list: run `skills_list` in Hermes, or check `~/.hermes/skills/`)*

---

## 3. Reason for each major decision

| Decision | Reason |
|----------|--------|
| Hermes as the agent (not Magpie) | Khairi's explicit choice; direct ChatGPT/Codex engine preferred |
| Claude as primary model | Best balance of speed and reasoning for his work streams |
| GPT-6 Luna as second opinion | Different company's model catches different blind spots |
| BM–English mixed interface | Natural for Khairi; Malay for cafe/admin, English for academic |
| No automatic posting on Threads/Crema | Hanani's override; Crema automation stays on-demand only |
| Local Ollama for llmbot | Privacy; local models stay on the Mac |
| Backups at 08:04 and 20:04 KL, keep 5 runs | Protects work without filling disk |

---

## 4. Interface (what the user sees)

- **Hermes desktop app** — main chat window. Type a goal, get a plan.
- **Model selector** — fast / standard / deep / second opinion
- **Work boards** — kanban-style boards where multi-step tasks move (To do → Running → Done)
- **Logs** — `~/.hermes/logs/hermes/*.md` — session records (read-only for the user)
- **Skills folder** — `~/.hermes/skills/` — each skill is a folder with SKILL.md

**Key screens:**
1. Chat input: "Give me one goal."
2. Plan view: Hermes shows the route before doing work.
3. Board view: tasks moving across columns (watch-only unless you approve).

---

## 5. Reasoning (how Hermes thinks, in plain words)

1. **You set a goal.** (e.g. "Plan my Chapter 4 analysis")
2. **Hermes plans.** It splits the goal into tasks and picks the right model level.
3. **Delegation.** Simple tasks → fast model. Hard tasks → deep model on a named work board.
4. **Second opinion.** For important plans, a different company's model (GPT-6 Luna) critiques it. Another bot (ultron) argues against it.
5. **Revision.** The drafting model fixes what's valid from the critique.
6. **You decide.** You get the plan, the critiques, and the open questions. Nothing happens without your OK.

**Guardrails (never without your OK):**
- Posting, messaging, or emailing as you
- Paid spend or new paid models
- Deleting anything (archive, not delete)
- Research data and citations (never invented)
- Patient, staff, and business figures (stay private)

---

## 6. Setup (step-by-step for the recipient)

### Step A — Get Hermes
1. Download the Hermes desktop app from [link / contact Dr Khairi].
2. Install on your Mac.
3. Log in with the account provided. (Do not create your own.)

### Step B — Connect Claude
- Claude is pre-connected inside Hermes.
- Choose model level per task: fast (Haiku), standard (Sonnet), deep (Opus).

### Step C — Add specialist bots (optional)
- To add a bot for your own work stream: ask Dr Khairi, or use the skill `create-specialist-bot`.
- Each bot needs: name, one job, memory location, model level.

### Step D — Set up local AI (optional, for privacy)
- Install Ollama on Mac.
- Pull a small model (e.g. `ollama pull llama3`).
- Hermes routes to it via llmbot when you choose "local/private".

### Step E — Guardrails
- Confirm: Hermes will ask before posting, spending, or deleting.
- Set your preference: archive instead of delete.

### Step F — First task
Send: "Hello Hermes. I'm new. Plan my week."

---

## 7. Files and folders

| Path | What's there |
|------|-------------|
| `~/.hermes/` | Hermes home (skills, plugins, cron, memories, logs, outputs) |
| `~/.hermes/skills/` | Installed skills (each is a folder with SKILL.md) |
| `~/.hermes/logs/hermes/` | Session logs |
| `~/.hermes/outputs/` | Finished deliverables (PDFs, HTML, reports) |
| `~/.hermes/cache/scratch` | Temporary files (pruned after 24h) |
| `~/projects/crema-site` | Crema Cafe website source (Cloudflare Pages) |

---

## 8. What to do when something breaks

| Symptom | First thing to try |
|---------|-------------------|
| Hermes doesn't reply | Check internet; restart the app |
| Wrong model used | Re-send with "use [fast/standard/deep] level" |
| Bot not responding | Ask Dr Khairi; check `~/.hermes/logs/hermes/` |
| Skill missing | Run `skills_list`; if absent, ask to install |
| Blender render needed | Blender isn't on this Mac — render elsewhere and drop .mp4/.webm into the slot |

---

## 9. Contact

- **Dr Mohd Khairi Safwan bin Johari** — drkhairisafwan@outlook.com
- **Crema Cafe:** @crema.kupisejuk (Instagram)
- **Hermes support:** check `~/.hermes/logs/hermes/` first, then message Dr Khairi

---

*Template end. Fill bracketed fields, delete this note, and hand over.*
