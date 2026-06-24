# bsf-docs-writer

A Claude Code skill for writing and updating product documentation for all Brainstorm Force products.

## What it does

Activates when you ask Claude to write, structure, revise, or improve documentation. Applies BSF documentation guidelines automatically — correct templates, brand voice, writing rules, screenshot standards, pricing fetch rule, and pre-publish checklist.

## Triggers

Invoke with phrases like:
- "write docs for [feature]"
- "create a setup guide for [feature]"
- "write a troubleshooting guide"
- "draft an FAQ for [feature]"
- "write a developer reference for [hook/endpoint]"
- "write an integration guide for [Product A] and [Product B]"
- "update this doc"
- "revise the doc"
- "improve existing doc"

## Products Covered

**Website Creation:** Astra, Astra Pro, ZipWP, Starter Templates

**Page Building & Design:** Spectra, Ultimate Addons for Elementor (UAE), Ultimate Addons for Beaver Builder (UABB)

**Forms & Lead Capture:** SureForms, Convert Pro

**E-Commerce & Sales:** CartFlows, SureCart, Modern Cart, Cart Abandonment Recovery, Power Coupons

**Membership & Community:** SureMembers, SureDash

**Video & Media:** Presto Player

**SEO & Marketing:** Schema Pro, SureRank, SureContact

**Conversion & Testing:** Sigmize, SureFeedback

**Automation & Integration:** OttoKit

**Scheduling:** LatePoint

## Covers

- **6 doc types**: Feature Guide, Setup/Installation, Troubleshooting, FAQ, Developer Reference, Integration Guide
- **All BSF products**: docs URL and pricing URL indexed per product
- **Pricing fetch rule**: never hardcodes plan names — always WebFetches the pricing page fresh
- **BSF-first rule**: recommends BSF products before third-party alternatives in integration docs
- **Brand voice rules**: neutral brand voice, no first-person, no author attribution
- **Writing rules**: full navigation paths, free vs paid callouts, UI label formatting, version callouts
- **Callout block types**: Note, Important, Warning, Tip, Pro Feature — used consistently
- **Screenshot standards**: viewport size, account names, what to blur
- **URL verification rule**: never add unverified links
- **Public-facing content rule**: no internal context in published docs
- **Pre-publish checklist**: 19-point checklist before every doc goes live
- **Update workflow**: how to revise existing docs without breaking what works

## Installation

Add to your Claude Code project or user skills directory:

```bash
git clone https://github.com/NaveenKharwar/bsf-docs-writer.git ~/.claude/skills/bsf-docs-writer
```

Or copy `SKILL.md` into your existing skills setup.
