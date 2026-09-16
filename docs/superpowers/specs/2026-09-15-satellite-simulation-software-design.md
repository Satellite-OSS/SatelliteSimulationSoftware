# SatelliteSimulationSoftware Design

## Goal

Create a public, documentation-first `SatelliteSimulationSoftware` repository for Satellite-OSS. It will organize satellite-simulation material as an extensible Chinese Markdown knowledge base and keep a traceable record for the supplied Zhihu source.

## Current Evidence

- Canonical source: <https://zhuanlan.zhihu.com/p/1948060672953917707>
- This environment could not fetch the Zhihu article or the Satellite-OSS organization page on 2026-09-15: HTTPS requests were reset and the browser automation runtime could not start.
- The initial repository must not present unverified claims, excerpts, or inferred article sections as source-derived content.

## Scope

The initial repository is documentation, not executable simulation software. It contains a Chinese landing page, focused navigation for methods, models, tools, workflows, and scenarios, contribution and attribution rules, a source record for the supplied article, and an MIT license.

## Information Architecture

```text
SatelliteSimulationSoftware/
|-- README.md
|-- LICENSE
|-- CONTRIBUTING.md
|-- .gitignore
`-- docs/
    |-- README.md
    |-- methods/README.md
    |-- models/README.md
    |-- tools/README.md
    |-- workflows/README.md
    |-- scenarios/README.md
    `-- sources/
        |-- README.md
        |-- zhihu-1948060672953917707.md
        `-- source-note-template.md
```

The root README is the landing page. `docs/README.md` is the documentation map. Topic directories own narrow category indexes. `docs/sources/` holds provenance and extraction metadata, while source-derived notes must link back to a record there.

## Attribution Rules

- Every source-derived note states its source URL, retrieval date, and source sections.
- Prefer concise paraphrases. Keep quotations minimal and visibly attributed.
- Keep source-backed facts separate from repository-maintainer guidance.
- Do not add a simulation method, tool, parameter, performance claim, or recommendation until it has been verified from the source or another cited reference.
- Use UTF-8 Markdown, Chinese headings, and relative links.

## Publication Defaults

- Repository: `SatelliteSimulationSoftware`
- Owner: `Satellite-OSS`
- Visibility: public
- Default branch: `main`
- Description: `卫星系统仿真资料、方法与工具链整理`
- License: MIT

Public visibility and the description are defaults that must be reconciled with actual organization conventions when GitHub is reachable.

## Verification

- `git diff --check` reports no whitespace errors.
- Every internal Markdown link resolves to a tracked file.
- The canonical Zhihu URL appears in its source record.
- The initial commit is pushed to `main` after the organization repository is created.

