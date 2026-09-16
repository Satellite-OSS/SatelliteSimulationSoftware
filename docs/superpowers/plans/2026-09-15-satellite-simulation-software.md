# SatelliteSimulationSoftware Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Build and publish a Chinese, source-traceable satellite-simulation knowledge-base repository named `SatelliteSimulationSoftware`.

**Architecture:** Use Markdown-only documentation with a root landing page and topic indexes under `docs/`. The supplied Zhihu URL is initially recorded as provenance rather than converted into claims until its article body is retrieved and reviewed.

**Tech Stack:** Git, GitHub, CommonMark-compatible Markdown.

**Spec:** `docs/superpowers/specs/2026-09-15-satellite-simulation-software-design.md`

## Global Constraints

- Owner is `Satellite-OSS`, repository name is exactly `SatelliteSimulationSoftware`, visibility is public, and default branch is `main`.
- Documentation is UTF-8 Markdown with Chinese headings and relative links.
- The canonical source URL is `https://zhuanlan.zhihu.com/p/1948060672953917707`.
- Do not claim article-derived content before it has been verified.
- License is MIT.

---

### Task 1: Establish Repository Identity

**Files:**
- Create: `README.md`
- Create: `LICENSE`
- Create: `CONTRIBUTING.md`
- Create: `.gitignore`

**Interfaces:**
- Consumes: publication defaults from the design specification.
- Produces: the landing page, contributor rules, license, and ignore policy referenced by later documentation.

- [ ] **Step 1: Add the landing page**

Create `README.md` with the title, the description `卫星系统仿真资料、方法与工具链整理`, links to `docs/README.md` and `CONTRIBUTING.md`, and a note that source-derived content is cited at the note level.

- [ ] **Step 2: Add repository policies**

Create `LICENSE` with the standard MIT text and `Copyright (c) 2026 Satellite-OSS`. Create `CONTRIBUTING.md` requiring a source link, retrieval date, concise paraphrase, and a source record for external material. Create `.gitignore` for `.DS_Store`, `Thumbs.db`, and editor swap files.

- [ ] **Step 3: Verify and commit**

Run:

```bash
git diff --check
git add README.md LICENSE CONTRIBUTING.md .gitignore
git commit -m "docs: initialize satellite simulation knowledge base"
```

Expected: no whitespace errors and one identity-layer commit.

### Task 2: Build Documentation Navigation

**Files:**
- Create: `docs/README.md`
- Create: `docs/methods/README.md`
- Create: `docs/models/README.md`
- Create: `docs/tools/README.md`
- Create: `docs/workflows/README.md`
- Create: `docs/scenarios/README.md`

**Interfaces:**
- Consumes: root README link target and category structure from the design specification.
- Produces: topic entry points for future source-derived notes.

- [ ] **Step 1: Add the documentation map**

Create `docs/README.md` with a table of the five categories and a relative link to each category index.

- [ ] **Step 2: Add focused category indexes**

Create one README per category. Each must state its scope, require citations for collected material, and link back to `docs/README.md`.

- [ ] **Step 3: Verify and commit**

Run:

```bash
git diff --check
git add docs/README.md docs/methods/README.md docs/models/README.md docs/tools/README.md docs/workflows/README.md docs/scenarios/README.md
git commit -m "docs: add simulation knowledge map"
```

Expected: no whitespace errors and one navigation-layer commit.

### Task 3: Add Zhihu Provenance

**Files:**
- Create: `docs/sources/README.md`
- Create: `docs/sources/zhihu-1948060672953917707.md`
- Create: `docs/sources/source-note-template.md`

**Interfaces:**
- Consumes: the canonical Zhihu URL and the attribution rules.
- Produces: a stable source record and a template that later notes reference.

- [ ] **Step 1: Add the source index and record**

Create a source table linking the supplied Zhihu record and label it `待读取原文`. The record must contain the canonical URL, the supplied sharing URL, retrieval status, retrieval date, source sections, validated summary, and destination notes. Leave factual summary sections empty until the source is read.

- [ ] **Step 2: Add the reusable source-note template**

Include fields for source URL, retrieval date, source sections, content type, destination category, and maintainer. Include headings for concise summary, verified claims, and related notes.

- [ ] **Step 3: Verify and commit**

Run:

```powershell
rg -n -F 'https://zhuanlan.zhihu.com/p/1948060672953917707' docs/sources/zhihu-1948060672953917707.md
git diff --check
git add docs/sources
git commit -m "docs: track Zhihu simulation source"
```

Expected: one canonical URL match, no whitespace errors, and one source-layer commit.

### Task 4: Publish to Satellite-OSS

**Files:**
- Modify: repository Git configuration only.

**Interfaces:**
- Consumes: committed local `main` branch.
- Produces: public `Satellite-OSS/SatelliteSimulationSoftware` with its local history pushed to `main`.

- [ ] **Step 1: Create the organization repository**

In a shell where `GITHUB_TOKEN` holds a token authorized to create Satellite-OSS repositories, run:

```powershell
$body = @{ name = 'SatelliteSimulationSoftware'; description = '卫星系统仿真资料、方法与工具链整理'; private = $false; has_issues = $true; has_projects = $true; has_wiki = $false; auto_init = $false } | ConvertTo-Json
Invoke-RestMethod -Method Post -Uri 'https://api.github.com/orgs/Satellite-OSS/repos' -Headers @{ Authorization = "Bearer $env:GITHUB_TOKEN"; Accept = 'application/vnd.github+json'; 'X-GitHub-Api-Version' = '2022-11-28' } -ContentType 'application/json' -Body $body
```

Expected: `full_name` is `Satellite-OSS/SatelliteSimulationSoftware` and `private` is `False`.

- [ ] **Step 2: Push the main branch**

Run:

```bash
git remote add origin https://github.com/Satellite-OSS/SatelliteSimulationSoftware.git
git push -u origin main
git ls-remote --heads origin main
```

Expected: the final command returns one line ending in `refs/heads/main`.

