# bsf-docs-writer

A Claude Code skill for writing and updating product documentation for Brainstorm Force products — Astra, Astra Pro, Spectra, Starter Templates, ZipWP, SureCart, and related products.

## What it does

Activates when you ask Claude to write, structure, revise, or improve documentation. Applies BSF documentation guidelines automatically — correct templates, brand voice, writing rules, screenshot standards, and pre-publish checklist.

## Triggers

Invoke with phrases like:
- "write docs for [feature]"
- "create a setup guide for [feature]"
- "write a troubleshooting guide"
- "draft an FAQ for [feature]"
- "update this doc"
- "revise the doc"
- "improve existing doc"

## Installation

Add to your Claude Code project or user skills directory:

```bash
git clone https://github.com/NaveenKharwar/bsf-docs-writer.git ~/.claude/skills/bsf-docs-writer
```

Or copy `SKILL.md` into your existing skills setup.

## Covers

- **4 doc types**: Feature Guide, Setup/Installation, Troubleshooting, FAQ
- **Brand voice rules**: neutral brand voice, no first-person, no author attribution
- **Writing rules**: full navigation paths, free vs pro callouts, UI label formatting
- **Screenshot standards**: viewport size, account names, what to blur
- **URL verification rule**: never add unverified links
- **Public-facing content rule**: no internal context in published docs
- **Pre-publish checklist**: 15-point checklist before every doc goes live
- **Update workflow**: how to revise existing docs without breaking what works
