---
name: bsf-docs-writer
description: >
  BSF product documentation writer for wpastra.com/docs and surecart.com/docs. Use this skill when writing, structuring, or improving documentation for Astra, Astra Pro, Spectra, Starter Templates, ZipWP, SureCart, or any other Brainstorm Force product. Triggers on requests like "write docs for", "create documentation", "write a guide for", "draft a setup doc", "write a feature guide", "create a troubleshooting guide", "write an FAQ", "update this doc", "revise the doc", "improve existing doc", or any request to document or update a BSF product feature or flow.
---

# BSF Documentation Writer

This skill helps write well-structured, consistent product documentation for Brainstorm Force products, following the official BSF Documentation Guidelines.

## Products Covered

- Astra (free theme)
- Astra Pro (premium addon)
- Spectra (free + pro Gutenberg blocks)
- Starter Templates
- ZipWP
- SureCart
- SureMembers, SureForms, SureRank, OttoKit (when relevant)

## Audience

Docs are written for WordPress users by default — non-technical or moderately technical audiences unfamiliar with internal terminology. Always write for the beginner first, then add advanced notes where needed. Never assume the user knows where to find a setting — always describe the full navigation path.

---

## Brand Voice Rules

Documentation must sound like it was written by the brand, not by an individual.

**Avoid first-person language:**
- ❌ "I suggest…"
- ❌ "We recommend…"

**Use neutral, recommendation-based language:**
- ✅ "It's recommended to…"
- ✅ "Best practices suggest…"
- ✅ "This approach helps ensure…"

For step-by-step instructions, second person ("you", "your site") is fine and preferred — but introductions, notes, and explanations should use neutral brand voice.

**Never identify the author.** No author names in content. Screenshots must not show personal usernames — use "BSF Docs", "SureCart Docs", or "John Doe" as the account name.

---

## Single-Purpose Rule

Each document must have exactly one clear goal:
- Explaining how something works, OR
- Guiding users through a task, OR
- Helping troubleshoot a specific problem

Never mix multiple objectives in one document.

---

## Step 0: New Doc or Update?

Before doing anything else, determine which applies:

- **Update existing doc** if: the request references an existing doc (by URL, title, or pasted content), uses words like "update," "revise," "improve," "fix," or "add to," or the person shares content that already exists on wpastra.com/docs or surecart.com/docs.
- **New doc** if: no existing doc is referenced, and the request is clearly asking for something that doesn't exist yet.
- **If unclear, ask before proceeding.** Do not default to writing a new doc when there's any chance an existing doc should be updated instead — regenerating a doc from scratch when an update was intended discards working content, screenshots, and structure unnecessarily.

Route to the matching workflow below ("Workflow: How to Write a Doc" or "Workflow: How to Update an Existing Doc").

---

## Flagging Uncertainty for the Reviewer

Never silently publish a step, setting description, or behavior as confirmed fact when it hasn't actually been verified (e.g., the UI location was inferred rather than checked directly, or the behavior may differ by version, plan tier, or configuration).

**When uncertain about a single detail**, flag it inline for manual verification:

> **⚠️ Verify before publishing:** This step assumes [specific assumption]. Please confirm manually.

**When the correct wording depends on something that can't be verified** (version, plan tier, active modules, config state), don't guess and pick one. Spell out the branches explicitly so the reviewer can choose the right one before publishing:

> **⚠️ Verify before publishing:** The exact behavior here depends on [condition].
> - If [condition A], keep this paragraph as-is: "[paragraph]"
> - If [condition B], replace with: "[alternate paragraph]"

These flags are for the human reviewer only and must never ship to the published doc. Before finalizing, confirm every flag has been resolved and removed.

---

## Doc Types & Their Structure

### 1. Feature Guide (How to Use a Feature)

```
# [Feature Name]

[1-2 sentence intro: what this feature does. Neutral brand voice — no "we".]

## Requirements
- WordPress version: X.X+
- [Product] version: X.X+
- [Free vs Pro — be explicit here, not buried later]

## How to Enable / Access
[Full navigation path. Example: Go to Appearance > Astra Options > ...]

## Step-by-Step

1. [Action]
2. [Action]
   - Sub-note if needed
3. [Action]

## Expected Outcome
[What the user should see or experience after completing the steps.]

## Settings Explained
[Flat-level bullet list with short descriptions of each option]

## Video Tutorial
[Screenshot: placeholder or embed note]

## Notes or Limitations (Optional)
[Known edge cases, limitations, or common mistakes]

## Related Docs
- [Link to related doc]

## FAQ (Optional — behavioral questions and edge cases only)

**Q: What happens if…**
A: [Short, objective answer]
```

---

### 2. Setup / Installation Doc

```
# Setting Up [Feature/Plugin]

[Brief intro — one clear goal: what this sets up and what the user will achieve. Neutral brand voice.]

## Requirements
- WordPress version: X.X+
- [Product] version: X.X+
- [Any other dependency]

## Installation Steps

1. Go to **WordPress Dashboard → Plugins → Add New**.
2. [Step]
3. [Step]

## Configuration

[Walk through each setting the user needs to configure after install. Full navigation paths for every setting.]

## Expected Outcome
[What the user should see when setup is complete.]

## Video Walkthrough
[Screenshot placeholder or embed note]

## Notes or Limitations (Optional)

## Troubleshooting
[Link to troubleshooting doc or 2-3 most common issues inline]

## Related Docs
- [Link]
```

---

### 3. Troubleshooting Guide

```
# Troubleshooting: [Issue or Feature Name]

[1-sentence description of what problems this doc addresses. Neutral brand voice.]

## Before You Begin
- Clear cache (site cache + browser cache)
- Disable other plugins temporarily to rule out conflicts
- Confirm the latest version of [product] is installed

## Common Issues

### Issue: [Problem Title]
**Symptom:** [What the user sees]
**Cause:** [Why it happens]
**Fix:**
1. [Step]
2. [Step]

**Expected outcome:** [What should happen after the fix]

### Issue: [Problem Title]
...

## Still Not Resolved?
If the above steps don't help, reach out to the [support team](https://wpastra.com/support/) with the following details:
- WordPress version
- [Product] version
- Steps to reproduce
- Screenshot or screen recording
```

---

### 4. FAQ Page

FAQs are for **behavioral questions and edge cases only** — not step-by-step instructions. Use them when:
- The feature has known limitations
- The behavior may change after updates
- Users may attempt unsupported workflows
- Support repeatedly receives the same question

```
# Frequently Asked Questions: [Topic/Feature]

**Q: What happens if…**
A: [Short, objective answer. No marketing language.]

**Q: Why does…**
A: [Explain the behavior clearly.]

**Q: Can I…**
A: [Yes/No + what to do next.]

**Q: What should I do if…**
A: [Practical next step.]
```

**Avoid:**
- Vague or generic questions
- Questions that restate the main steps
- Marketing language or reassurance-only answers ("Don't worry, this is easy!")

---

## Writing Rules

### Tone & Voice
- Neutral brand voice for introductions, notes, and explanations.
- Second person ("you", "your site") for step-by-step instructions.
- Active voice. "Click **Save**" not "The Save button should be clicked."
- No filler openers: "In this article, we will…" → just start.
- No superlatives: "best", "powerful", "amazing" — explain instead of promoting.
- Documentation should explain, not sell.

### Clarity
- Every step must be actionable. If it's not something the user *does*, it's not a step.
- Always give the **full navigation path**. Example: `WordPress Dashboard → SureCart → Products`.
- One term per concept. Don't alternate between "checkout", "checkout page", and "checkout form" — pick one and use it consistently throughout, matching the UI label exactly.
- When a feature requires **Astra Pro** (or any paid plan), call it out clearly at the top under Requirements — never buried in the middle.
- Use **bold** for UI labels exactly as they appear in the interface (e.g., **Save Changes**, **Enable**, **Typography**).
- Use `code formatting` for file paths, shortcodes, CSS snippets, filter/hook names.
- Before a set of steps addressing a common task, add a bridging sentence phrased the way a user would ask it, e.g. "If you're looking to disable the sticky header, follow the steps below…" This improves the match between how users phrase questions and the retrieved content.
- Define acronyms and product-specific terms on first use in a document (e.g. "UAE (Ultimate Addons for Elementor)", "HFE", "WPML"). Don't assume context carries over from another document or an earlier section.

### Structure
- Use H2 for major sections, H3 for sub-sections. Never skip heading levels.
- Steps go in numbered lists. Options/settings go in flat-level bullet lists — never tables. Tables require understanding two-dimensional structure that retrieval systems can't reliably preserve when a document is chunked.
- Numbered lists must stay strictly sequential, never skip numbers, even across edits.
- Where steps depend on each other, add a short transition phrase ("After completing step 2, do…") so a retrieved chunk still makes sense in isolation.
- For docs longer than roughly three H2 sections (Feature Guide, Troubleshooting, Setup docs), open each H2 with a 1–2 sentence summary of what that section covers, before diving into steps or details.
- Group related settings together — don't list them in random order.
- Most common use case first. Edge cases go at the bottom or in a Notes section.
- Always include an **Expected Outcome** section after steps so users can confirm it worked.

### Screenshots
- Viewport: **1280×800px** (set via browser dev tools).
- Clean WordPress install — only required plugins active, no unrelated plugins visible in menus or UI.
- Account name in screenshots: use **BSF Docs**, **SureCart Docs**, or **John Doe**. Never personal usernames.
- Always blur or remove: API keys, tokens, email addresses, account identifiers.
- Upload screenshots directly to WordPress — never embed from Google Docs or external hosts.
- Screenshots support the text, they don't replace it. Never write "as shown in the image" — the text must stand alone. The surrounding text must fully describe what the screenshot shows (the setting, its location, and the result), not just reference it — image content isn't reliably captured by automated retrieval systems.
- If removing a screenshot doesn't reduce clarity, it's unnecessary.

### Media Placeholders
When screenshots or videos are needed, add a placeholder:
- `[Screenshot: Show location of X setting — WordPress Dashboard → Product → Tab]`
- `[Video: Walkthrough of setting up X from scratch]`

Don't skip these — they're reminders for the publishing step.

### Free vs Pro Callouts
Always be explicit. Use a note block:
> **Note:** This feature requires **Astra Pro**. [Upgrade here](https://wpastra.com/pricing/).

Or for free features:
> **Note:** This feature is available in the **free version** of Astra.

---

## URL Verification Rule

**Never add a URL to a doc without verifying it first.** This applies to all links — related docs, support pages, pricing pages, upgrade links, or any external reference.

Before including any link:
1. **Fetch the URL** using the web fetch tool and confirm the page exists and contains the content you expect.
2. If the page returns a 404, redirects somewhere unrelated, or doesn't exist — **do not include the link.** Use a placeholder instead: `[Link: page name — URL to be confirmed]`
3. Never guess or construct a URL based on a pattern (e.g., assuming `/docs/feature-name/` exists just because similar URLs do).

This applies equally when **updating existing docs** — if a linked URL was added previously, verify it still resolves correctly before leaving it in.

❌ Adding `https://wpastra.com/docs/wpml-compatibility/` without checking if that page exists  
✅ Fetching the URL first, confirming it loads the right content, then including it

---

## Public-Facing Content Rule

Documentation is read by end users — not internal team members. **Never include internal context in public docs.** This includes:

- Explanations of why a core fix wasn't possible (e.g., "due to a conflict between X and Y, a core fix would introduce a regression")
- References to GitHub issues, internal Slack discussions, or sprint decisions
- Wordings that imply the fix is a compromise or a known limitation in the product
- Any language that could erode user trust in the product

**Instead:** Present the fix matter-of-factly. Users need to know *what to do* — not the internal trade-offs behind the decision.

❌ "Due to a conflict between how Astra loads default strings and how WPML manages the global locale stack, this issue cannot be resolved through a core theme update without introducing a separate regression…"

✅ "The recommended fix is a small code snippet added to your child theme. It ensures Astra uses the correct frontend language when loading Customizer strings…"

---

## Workflow: How to Write a Doc

1. **Identify the doc type** — feature guide, setup, troubleshooting, or FAQ.
2. **Confirm the single goal** — if there are multiple goals, split into separate docs.
3. **Ask for missing info** if the feature name or context is unclear. Don't guess.
4. **Use the matching template** from above.
5. **Fill every section** — mark `[To be added]` if content isn't available yet.
6. **Add screenshot/video placeholders** wherever media would help.
7. **Run the pre-publish checklist** before finalizing.

---

## Workflow: How to Update an Existing Doc

Use this workflow when revising or improving an existing doc rather than writing from scratch.

1. **Read the existing doc in full** before making any changes. Understand what it currently covers.
2. **Identify what's changing** — new steps, removed steps, updated UI labels, changed navigation paths, deprecated features, added requirements, or structural improvements.
3. **Do not rewrite what isn't broken.** Preserve working sections, existing examples, and screenshot placeholders unless they're directly affected by the change.
4. **Update section by section** — don't replace the whole doc unless a full rewrite is explicitly requested.
5. **Flag anything that needs a new screenshot** — if a UI path or setting has changed, add or update the screenshot placeholder.
6. **Check consistency** — after updating, verify that terminology is still consistent throughout the whole doc (not just the updated section).
7. **Run the pre-publish checklist** on the full doc, not just the changed parts.

---

## Pre-Publish Checklist

- [ ] Confirmed whether this is a new doc or an update to an existing one before starting (Step 0)
- [ ] No unresolved ⚠️ verification flags remaining — every uncertain step or branch has been confirmed and cleaned up
- [ ] Single clear goal — no mixed objectives
- [ ] Neutral brand voice (no "I", "we", no author name)
- [ ] No internal context exposed (no GitHub issues, Slack references, regression mentions, or internal trade-off explanations)
- [ ] Full navigation paths on every setting
- [ ] Free vs Pro requirement stated at the top
- [ ] All steps numbered, actionable, and strictly sequential (no skipped numbers)
- [ ] Transition phrases added between dependent steps or list items
- [ ] Each H2 section opens with a 1–2 sentence summary (for docs with 3+ H2 sections)
- [ ] No tables — settings/options presented as flat-level bullet lists
- [ ] Bridging "session starter" sentence included before steps addressing a common task
- [ ] Acronyms and product-specific terms defined on first use
- [ ] Expected Outcome section included
- [ ] UI labels bolded exactly as they appear in the interface
- [ ] Consistent terminology throughout (one term per concept)
- [ ] Screenshot placeholders added where needed, with surrounding text fully describing what each screenshot shows
- [ ] No filler intro ("In this doc we will…")
- [ ] No marketing language or superlatives
- [ ] Notes/limitations section included if relevant
- [ ] All URLs verified — fetched and confirmed to exist with correct content (no guessed or assumed links)
- [ ] FAQ uses behavioral questions only (if included)
