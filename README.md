# bsf-docs-writer

A documentation-writing skill for Brainstorm Force products (Astra, Astra Pro, Spectra, Starter Templates, ZipWP, SureCart, and others). It defines a consistent structure, tone, and set of writing rules for feature guides, setup docs, troubleshooting guides, and FAQs published on `wpastra.com/docs` and `surecart.com/docs`.

## Why this skill is structured this way

Several of this skill's structural rules (avoiding tables, sequential numbered lists, per-section summaries, defining abbreviations on first use, and bridging "session starter" sentences before common tasks) are informed by published guidance on writing documentation that retrieval-augmented systems can index and retrieve accurately:

- **AWS Prescriptive Guidance — [Writing best practices to optimize RAG applications](https://docs.aws.amazon.com/pdfs/prescriptive-guidance/latest/writing-best-practices-rag/writing-best-practices-rag.pdf)** (July 2025)

The core idea: documentation written purely for human reading doesn't always retrieve well in automated systems, since content gets split into smaller chunks and retrieved based on semantic similarity to a query. Structure that seems redundant to a human reader (a summary at the top of every section, defining an acronym you'd expect a reader to already know, avoiding two-dimensional tables) meaningfully improves how reliably the right information gets surfaced.

## What's in SKILL.md

- Doc types and their required structure (Feature Guide, Setup/Installation, Troubleshooting, FAQ)
- A gate for deciding whether a request is a new doc or an update to an existing one, so existing docs aren't regenerated from scratch by mistake
- A rule for flagging uncertain or version/plan-dependent steps for manual review, rather than silently guessing
- Brand voice and tone rules
- Formatting rules (headings, lists, screenshots, free vs. pro callouts)
- A URL verification rule (never link without fetching and confirming first)
- A public-facing content rule (no internal context, GitHub issues, or Slack references in published docs)
- Workflows for writing new docs and updating existing ones
- A pre-publish checklist

## Usage

This is a Claude Skill. Drop the `SKILL.md` file into a skills directory the model can read, and it activates on requests like "write docs for X," "update this doc," or "create a troubleshooting guide for Y."
