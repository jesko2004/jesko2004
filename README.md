<div align="center">

# Andy Dai

### AI Application Developer

**RAG · AI Agents · Workflow Engineering · Model Evaluation**

I build document intelligence systems and dependable AI workflows with clear boundaries, traceable evidence, and measurable quality.

[![GitHub](https://img.shields.io/badge/GitHub-jesko2004-181717?style=flat-square&logo=github)](https://github.com/jesko2004) [![Primary Project](https://img.shields.io/badge/Primary_Project-PDF_Inspector-0A7EA4?style=flat-square)](https://github.com/jesko2004/pdf-inspector) [![Open Source](https://img.shields.io/badge/Open_Source-Contributor-2EA44F?style=flat-square&logo=github)](https://github.com/jesko2004#open-source-contributions) [![Focus](https://img.shields.io/badge/Focus-Document_AI_%26_RAG-6F42C1?style=flat-square)](https://github.com/jesko2004/pdf-inspector)

</div>

---

## Selected Work

<table>
<tr>
<td width="50%" valign="top">

### PDF Inspector

**Core Project Lead · Completed**

A Rust-centered toolkit that classifies PDFs, extracts layout-aware content, and produces structured Markdown or JSON. Its optional local backend adds OCR routing, business-field extraction, knowledge-base retrieval, cited answers, auditing, and backup recovery.

**My ownership**

- Led the architecture and end-to-end delivery.
- Developed the PDF processing, OCR, and RAG workflow.
- Delivered Rust, Python, Node.js, WASM, CLI, and FastAPI interfaces.
- Drove regression fixes, acceptance testing, and project documentation.

`Rust` `Python` `FastAPI` `PyO3` `WASM` `SQLite` `RapidOCR` `RAG`

**Evidence:** 893 Rust tests, 95 backend tests, 16 PDFs / 86 pages, and 22 end-to-end recovery checks recorded in the final acceptance scope.

[View repository →](https://github.com/jesko2004/pdf-inspector)

</td>
<td width="50%" valign="top">

### MergeWarden

**Tools & Integration Module Owner · Contributor**

An advisory AI Pull Request reviewer that turns diffs, repository context, tests, and CI logs into evidence-backed findings and practical repair guidance.

**My contribution**

- Connected the CLI to the orchestration layer.
- Built the initial read-only tool chain: file read, glob, grep, and directory listing.
- Added sandboxed command execution, permission modes, and path-boundary controls.
- Improved cross-platform tests, typing, evaluation fixtures, and finding triage.

`Python` `CLI` `Pydantic` `JSON Schema` `Sandboxing` `pytest` `mypy`

[View repository →](https://github.com/takagibit18/MergeWarden) · [My commits →](https://github.com/takagibit18/MergeWarden/commits/main/?author=jesko2004)

</td>
</tr>
</table>

---

## Current Build

I am refining **PDF Inspector** into a dependable local-first document intelligence foundation while contributing focused compatibility and reliability fixes to **JiraTUI**, **Rainfrog**, **tldextract**, and **Microsoft MarkItDown**.

`Document AI` `Local-first RAG` `Reliable Agent Tools` `Open Source`

---

## Open Source Contributions

<table>
<tr>
<td width="50%" valign="top">

### [Rainfrog](https://github.com/achristmascarl/rainfrog) · 5.3k+ Stars

**Contributor · Merged PR #344**

A Rust terminal database tool for editing SQL, running queries, and browsing results.

**My contribution**

- Fixed SQL syntax highlighting that skipped adjacent keywords because the regex consumed the separator after each match.
- Used a non-consuming word boundary to preserve highlighting across consecutive keywords.
- Added a rendering regression test with Ratatui TestBackend to verify the actual highlighted characters.

**Validation:** 183 tests passed with `--no-default-features`; all 10 remote CI checks passed, including Windows, macOS, and Linux test suites.

`Rust` `Regex` `Ratatui` `Regression Tests` `GitHub Actions`

[Merged pull request →](https://github.com/achristmascarl/rainfrog/pull/344) · [Merged commit →](https://github.com/achristmascarl/rainfrog/commit/771fa61b86bc9a4838c952d729ba79319a556f33)

</td>
<td width="50%" valign="top">

### [tldextract](https://github.com/john-kurkowski/tldextract) · 2k+ Stars

**Contributor · Merged PR #383**

A Python library that separates URL subdomains, domains, and public suffixes using the Public Suffix List (PSL).

**My contribution**

- Reported a reproducible bug where an incomplete longer trie match discarded the private metadata of the suffix that actually matched.
- Preserved the last complete suffix node, correcting `is_private`, `registry_suffix`, and `top_domain_under_registry_suffix` results.
- Added seven offline regression cases covering incomplete matches, a complete longer match, a wildcard parent, and private suffix extraction disabled.

**Validation:** 118 tests passed with one Windows-specific skip; formatting, lint, and type checks passed. All 25 remote CI checks passed across Windows, macOS, Linux, CPython 3.10–3.14, and PyPy.

`Python` `Trie` `Domain Parsing` `pytest` `Ruff` `mypy`

[Resolved issue →](https://github.com/john-kurkowski/tldextract/issues/382) · [Merged pull request →](https://github.com/john-kurkowski/tldextract/pull/383) · [Merged commit →](https://github.com/john-kurkowski/tldextract/commit/89b9aebf6d9860cca2bd5fe6a5f3f506bb266363)

</td>
</tr>
<tr>
<td width="50%" valign="top">

### JiraTUI · 1.7k+ Stars

**Contributor · Merged PR #361**

Fixed a work-item details crash caused by Jira Server/Data Center returning Sprint fields as strings instead of Cloud-style objects.

**My contribution**

- Built a backward-compatible parser for Cloud JSON, scalar strings, list-wrapped values, and legacy Java-style Sprint representations.
- Extracted real Sprint names across field-order variations, including `rapidViewId`, `id`, and `state`, while preserving names containing commas.
- Confirmed the Cloud Sprint update path remained intact and the Server/DC field stayed safely read-only.
- Added regression coverage, passed the cross-platform CI matrix, and incorporated validation from a Jira Data Center 10.6 user.

`Python` `Regex` `Jira API` `Regression Tests`

[Merged pull request →](https://github.com/whyisdifficult/jiratui/pull/361) · [Merged commit →](https://github.com/whyisdifficult/jiratui/commit/b2bda27b62fb8ff92cf8b491a3f7ebf2806698d7)

</td>
<td width="50%" valign="top">

### Microsoft MarkItDown · PR #2543

**Standards-aware HTTP charset parsing**

Fixed `Content-Type` parsing when quoted parameters contain semicolons, preventing unrelated parameter text from overriding the real charset. Reused Python's standard email parser and added nine regression and control cases through the public conversion API.

`Python` `HTTP` `Content-Type` `Encoding` `pytest`

[View pull request →](https://github.com/microsoft/markitdown/pull/2543)

</td>
</tr>
</table>

---

## Engineering Profile

<table>
<tr>
<td width="33%" valign="top">

### AI Systems

I turn ambiguous requirements into bounded workflows with explicit inputs, tool permissions, structured outputs, and recovery paths.

</td>
<td width="33%" valign="top">

### Evidence & Evaluation

I keep source locations, confidence, tests, golden cases, and acceptance limits attached to important system claims.

</td>
<td width="33%" valign="top">

### Delivery

I include interfaces, documentation, CI, observability, security boundaries, backup, and reproducibility in the delivery scope.

</td>
</tr>
</table>

**Languages:** `Rust` `Python` `JavaScript`  
**AI & Data:** `RAG` `Agent Workflows` `OCR` `Document Parsing` `Model Evaluation`  
**Engineering:** `FastAPI` `SQLite` `Docker` `GitHub Actions` `pytest` `Ruff` `mypy`

<div align="center">

---

[GitHub](https://github.com/jesko2004) · [PDF Inspector](https://github.com/jesko2004/pdf-inspector) · [MergeWarden](https://github.com/takagibit18/MergeWarden)

</div>
