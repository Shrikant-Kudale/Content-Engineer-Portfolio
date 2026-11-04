<div align="center">

# 📂 Content Engineer Portfolio

**Technical writing and Generative AI, in one place.**
Four writing samples and two GenAI documentation tools, all written and built by me.

[![Writing Samples](https://img.shields.io/badge/Writing_Samples-View_on_GitHub-181717?style=for-the-badge&logo=github)](https://github.com/Shrikant-Kudale/Writing-Samples)
[![DriftWatch](https://img.shields.io/badge/DriftWatch-Live_Demo-3D5AFE?style=for-the-badge&logo=vercel&logoColor=white)](https://driftwatch-gen-ai.vercel.app/)
[![DocPilot](https://img.shields.io/badge/DocPilot-Live_Demo-0B7A75?style=for-the-badge&logo=vercel&logoColor=white)](https://docpilotgenaiproject.vercel.app/)

</div>

---

## 🗺️ At a Glance

| # | Project | What it is | Links |
|---|---|---|---|
| 1 | ✍️ **Writing Samples** | Four documents: research, academic, product and explanatory writing | [GitHub](https://github.com/Shrikant-Kudale/Writing-Samples) |
| 2 | 🛰️ **DriftWatch** | GenAI tool that finds stale docs after a product change | [Live](https://driftwatch-gen-ai.vercel.app/) · [GitHub](https://github.com/Shrikant-Kudale/DriftWatch-GEN-AI) |
| 3 | 🧭 **DocPilot** | GenAI workbench for technical writers | [Live](https://docpilotgenaiproject.vercel.app/) · [GitHub](https://github.com/Shrikant-Kudale/DocPilot---Tech-Writer-Workbench---GEN-AI-Project) |

---

## ✍️ 1. Writing Samples

Four samples I wrote myself, covering technical, academic, procedural and plain-language writing.

📁 **Repository:** [Shrikant-Kudale/Writing-Samples](https://github.com/Shrikant-Kudale/Writing-Samples)

| Sample | Type | What it shows | Read |
|---|---|---|---|
| **S1.** Neuro-Cognitive AI Fingerprinting for Pre-Radiographic Brain Tumor Detection | Technical documentation of a research paper | Structuring dense technical material, tables and workflow diagrams, honest scope-setting | [📄 PDF](https://github.com/Shrikant-Kudale/Writing-Samples/blob/main/S1_Neuro_Cognitive_AI_Fingerprinting_Technical_Documentation.pdf) |
| **S2.** AI Reliance, Spatial Memory and Subjective Forgetfulness | Shortened psychology dissertation | Academic tone, explaining statistics to a general reader, avoiding overclaiming | [📄 PDF](https://github.com/Shrikant-Kudale/Writing-Samples/blob/main/S2_Psychology_Dissertation_Sample.pdf) |
| **S3.** Safely Remove Old Restic Snapshots and Reclaim Repository Space | Product documentation, how-to procedure | Prerequisites, five tested steps, `--dry-run` safety, troubleshooting, works on PowerShell, macOS and Linux | [📄 PDF](https://github.com/Shrikant-Kudale/Writing-Samples/blob/main/S3_Restic_Safe_Snapshot_Cleanup.pdf) |
| **S4.** The Art of Explaining Complex Things Simply | Explanatory article | Clear voice, logical flow, audience awareness | [📄 PDF](https://github.com/Shrikant-Kudale/Writing-Samples/blob/main/S4_The_Art_Of_Explaining_Complex_Things_Simply.pdf) |

> S1 documents my published research: *IJARSCT, April 2026* · [DOI 10.48175/IJARSCT-34249](https://doi.org/10.48175/IJARSCT-34249). The research samples use simulated or self-reported data and make no clinical claims.

---

## 🛰️ 2. DriftWatch

> **"AI proposes. A human decides."**

[![Live](https://img.shields.io/badge/Live_Demo-driftwatch--gen--ai.vercel.app-3D5AFE?style=flat&logo=vercel&logoColor=white)](https://driftwatch-gen-ai.vercel.app/)
[![GitHub](https://img.shields.io/badge/Source-GitHub-181717?style=flat&logo=github)](https://github.com/Shrikant-Kudale/DriftWatch-GEN-AI)

- 🔗 **Live demo:** [https://driftwatch-gen-ai.vercel.app/](https://driftwatch-gen-ai.vercel.app/)
- 💻 **Source code:** [https://github.com/Shrikant-Kudale/DriftWatch-GEN-AI](https://github.com/Shrikant-Kudale/DriftWatch-GEN-AI)

When a product changes (a pull request, commit log or ticket), DriftWatch finds which documentation pages have gone stale and proposes surgical fixes. A person approves each fix before a Git patch is exported.

**How it works**
1. 🔒 Paste a change. A secret scanner removes API keys, tokens, emails and IPs first.
2. 🔎 The change is embedded and matched to doc chunks with cosine similarity (RAG).
3. ✍️ Gemini drafts minimal edits as strict JSON, each with a confidence level.
4. ✅ A human approves, rejects or edits each fix, then exports a `.patch`.

**Highlights**
- Side-by-side diffs with a mandatory verification checkbox before export
- Audience briefings for administrators, executives and support teams
- `scripts/drift_check.py` plus a GitHub Actions workflow that audit doc staleness on every PR
- Tracks engineering hours saved

**Stack:** React · TypeScript · Vite · Vercel serverless · Google Gemini · Python · GitHub Actions

---

## 🧭 3. DocPilot

> **AI documentation workbench for technical writers.**

[![Live](https://img.shields.io/badge/Live_Demo-docpilotgenaiproject.vercel.app-0B7A75?style=flat&logo=vercel&logoColor=white)](https://docpilotgenaiproject.vercel.app/)
[![GitHub](https://img.shields.io/badge/Source-GitHub-181717?style=flat&logo=github)](https://github.com/Shrikant-Kudale/DocPilot---Tech-Writer-Workbench---GEN-AI-Project)

- 🔗 **Live demo:** [https://docpilotgenaiproject.vercel.app/](https://docpilotgenaiproject.vercel.app/)
- 💻 **Source code:** [https://github.com/Shrikant-Kudale/DocPilot---Tech-Writer-Workbench---GEN-AI-Project](https://github.com/Shrikant-Kudale/DocPilot---Tech-Writer-Workbench---GEN-AI-Project)

DocPilot tackles three problems writers face with AI: invented details (hallucination), inconsistent style, and not knowing what readers ask that the docs don't answer.

**Modules**
- 💬 **Ask the Docs:** answers with numbered source citations, using hybrid retrieval (vector similarity plus BM25 keyword scoring)
- 📚 **Knowledge Base:** ingests PDF, Word, Markdown and text files into indexed chunks
- 🧹 **Style Linter:** flags passive voice, vague links, non-inclusive terms and steps that don't start with a verb, then suggests an AI fix
- ✏️ **Rewrite Assistant:** original and AI draft side by side, and export stays locked until a human ticks "Human verified"
- 🧪 **Prompt Lab:** compares two prompt versions on the same input, with a hallucination flag
- 📊 **Evaluation:** a golden question set scored on retrieval hit rate (Hit@3) and answer accuracy
- 🕳️ **Gap Report:** collects unanswered questions to show what to write next
- ⚙️ **Automation:** link checker, front matter validator and release-note assembler

**Stack:** React · TypeScript · Vite · Vercel serverless (API key stays server-side) · Google Gemini (generation and embeddings) · storage layer ready for Supabase pgvector

---

## 🎯 What This Portfolio Shows

| Skill | Where to see it |
|---|---|
| Technical and structured writing | Writing Samples S1 to S4 |
| Product documentation and procedures | S3 (Restic), DriftWatch doc edits |
| GenAI, prompt design, hallucination control | DriftWatch, DocPilot (Prompt Lab) |
| RAG, embeddings, semantic search | DriftWatch, DocPilot |
| Python and Git automation | DriftWatch (`drift_check.py`, GitHub Actions), DocPilot Automation |
| Human accuracy gate and data safety | DriftWatch (secret scanner, approval gate), DocPilot ("Human verified") |
| Markdown and docs-as-code | All three |

---

<div align="center">

**Shrikant Kudale** · Computer Science & Engineering, MIT School of Computing
🐙 [github.com/Shrikant-Kudale](https://github.com/Shrikant-Kudale)

</div>
