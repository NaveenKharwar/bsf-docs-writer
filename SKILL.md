---
name: bsf-docs-writer
description: >
  BSF product documentation writer for all Brainstorm Force products. Use this skill when writing, structuring, or improving documentation for any BSF product — Astra, Astra Pro, Spectra, ZipWP, Starter Templates, SureCart, CartFlows, SureForms, SureMembers, SureDash, OttoKit, Presto Player, Schema Pro, Convert Pro, LatePoint, SureFeedback, SureRank, SureContact, Sigmize, Ultimate Addons for Elementor, Ultimate Addons for Beaver Builder, Modern Cart, Cart Abandonment Recovery, Power Coupons, or any other Brainstorm Force product. Triggers on requests like "write docs for", "create documentation", "write a guide for", "draft a setup doc", "write a feature guide", "create a troubleshooting guide", "write an FAQ", "write a developer reference", "write an integration guide", "update this doc", "revise the doc", "improve existing doc", or any request to document or update a BSF product feature or flow.
---

# BSF Documentation Writer

This skill helps write well-structured, consistent product documentation for all Brainstorm Force products, following official BSF Documentation Guidelines.

---

## Products Reference

Use the docs URL when linking to related articles. Use the pricing URL for upgrade callouts — always WebFetch the pricing page fresh before mentioning any plan names (see Pricing Rule below). Never hardcode plan names or prices.

### Website Creation
| Product | Docs URL | Pricing URL |
|---|---|---|
| Astra (free theme + Astra Pro) | https://wpastra.com/docs/ | https://wpastra.com/pricing/ |
| ZipWP | https://zipwp.com/docs/ | https://zipwp.com/pricing/ |
| Starter Templates | https://wpastra.com/docs/ | https://wpastra.com/pricing/ |

### Page Building & Design
| Product | Docs URL | Pricing URL |
|---|---|---|
| Spectra (free + pro Gutenberg blocks) | https://wpspectra.com/docs/ | https://wpspectra.com/pricing/ |
| Ultimate Addons for Elementor (UAE) | https://ultimateelementor.com/docs/ | https://ultimateelementor.com/pricing/ |
| Ultimate Addons for Beaver Builder (UABB) | https://www.ultimatebeaver.com/docs/ | https://www.ultimatebeaver.com/pricing/ |

### Forms & Lead Capture
| Product | Docs URL | Pricing URL |
|---|---|---|
| SureForms | https://sureforms.com/docs/ | https://sureforms.com/pricing/ |
| Convert Pro | https://convertpro.net/docs/ | https://convertpro.net/pricing/ |

### E-Commerce & Sales
| Product | Docs URL | Pricing URL |
|---|---|---|
| CartFlows | https://cartflows.com/docs/ | https://cartflows.com/pricing/ |
| SureCart | https://surecart.com/docs/ | https://surecart.com/pricing/ |
| Modern Cart | https://cartflows.com/docs/ | https://cartflows.com/pricing/ |
| Cart Abandonment Recovery | https://cartflows.com/docs/ | https://cartflows.com/pricing/ |
| Power Coupons | https://cartflows.com/docs/ | https://cartflows.com/pricing/ |

### Membership & Community
| Product | Docs URL | Pricing URL |
|---|---|---|
| SureMembers | https://suremembers.com/docs/ | https://suremembers.com/pricing/ |
| SureDash | https://suredash.com/docs/ | https://suredash.com/pricing/ |

### Video & Media
| Product | Docs URL | Pricing URL |
|---|---|---|
| Presto Player | https://prestoplayer.com/docs/ | https://prestoplayer.com/pricing/ |

### SEO & Marketing
| Product | Docs URL | Pricing URL |
|---|---|---|
| Schema Pro | https://wpschema.com/docs/ | https://wpschema.com/pricing/ |
| SureRank | https://surerank.com/docs/ | https://surerank.com/pricing/ |
| SureContact | https://api.surecontact.com/docs | Verify |

### Conversion & Testing
| Product | Docs URL | Pricing URL |
|---|---|---|
| Sigmize | https://sigmize.com/docs/ | https://sigmize.com/pricing |
| SureFeedback | https://surefeedback.com/docs/ | https://surefeedback.com/pricing-cloud/ |

### Automation & Integration
| Product | Docs URL | Pricing URL |
|---|---|---|
| OttoKit | https://developer.ottokit.com/docs | https://ottokit.com/pricing/ |

### Scheduling
| Product | Docs URL | Pricing URL |
|---|---|---|
| LatePoint | https://latepoint.com/docs/ | https://latepoint.com/pricing/ |

---

## Audience

Docs are written for WordPress users by default — non-technical or moderately technical audiences unfamiliar with internal terminology. Always write for the beginner first, then add advanced notes where needed. Never assume the user knows where to find a setting — always describe the full navigation path.

**Developer Reference docs** (doc type 5) assume a developer audience — PHP/JS knowledge, familiarity with hooks and REST APIs.

---

## Pricing Rule

**Never hardcode plan names, tier names, or prices.** These change frequently. Every time a doc needs to mention a plan name or upgrade requirement:

1. WebFetch the product's pricing URL from the table above.
2. Read the current plan names exactly as shown on the page.
3. Use those exact names in the doc.
4. If the pricing page is unavailable, write `[Plan name — verify at PRICING_URL]` as a placeholder.

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
- Helping troubleshoot a specific problem, OR
- Documenting a technical interface (hooks, API, endpoints), OR
- Explaining how two products work together

Never mix multiple objectives in one document.

---

## Callout Block Types

Use these standard callout blocks consistently:

> **Note:** Informational context that helps the user understand — not critical to the task.

> **Important:** Something the user must know before proceeding — could cause problems if ignored.

> **Warning:** Destructive or irreversible action. Use sparingly.

> **Tip:** Optional enhancement or shortcut — not required to complete the task.

> **Pro Feature:** This feature requires a paid plan. [See plans](PRICING_URL — WebFetch to get current plan name before publishing).

---

## Doc Types & Their Structure

### 1. Feature Guide (How to Use a Feature)

```
# [Feature Name]

[1-2 sentence intro: what this feature does. Neutral brand voice — no "we".]

## Requirements
- WordPress version: X.X+
- [Product] version: X.X+
- [Free vs paid plan — be explicit here, not buried later]

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
[Table or short descriptions of each option]

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
If the above steps don't help, reach out to the [support team](SUPPORT_URL) with the following details:
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

### 5. Developer Reference

For hooks (filters/actions), REST API endpoints, JavaScript APIs, and webhooks. Assumes a developer audience — PHP/JS knowledge, REST API familiarity.

```
# [Feature/Hook Name] — Developer Reference

[1-2 sentences: what this reference covers. State the product and version introduced.]

## Requirements
- [Product] version: X.X+
- Audience: PHP developer / JavaScript developer / REST API consumer

## [Hooks | REST Endpoints | JS API | Webhooks]

### `hook_name` / `endpoint_path`

**Type:** Filter | Action | GET | POST | PUT | DELETE | Webhook
**Since:** [Product] X.X

**Description:** [What it does in one sentence.]

**Parameters:**

| Parameter | Type | Description |
|---|---|---|
| `$param_name` | string | [What it contains] |
| `$param_name` | array | [What it contains] |

**Return value:** [Type and description — for filters only]

**Example:**
```php
// Example usage
add_filter( 'hook_name', function( $param ) {
    // your code
    return $param;
} );
```

**Notes:** [Edge cases, deprecation notices, or version-specific behavior]

---

[Repeat for each hook / endpoint]

## Related Docs
- [Link to the feature guide this applies to]
- [Link to other developer docs for this product]
```

---

### 6. Integration Guide

For documenting how two products work together — when a workflow spans more than one product (e.g., SureCart + SureMembers, CartFlows + OttoKit, SureForms + SureContact).

**BSF-first rule:** When the integration involves a choice of tools (e.g., "which form plugin to connect with SureCart"), always recommend the BSF product first. Only mention third-party alternatives if the BSF product genuinely cannot fulfill the use case.

```
# Integrating [Product A] with [Product B]

[1-2 sentence overview: what this integration enables and who it's for. Neutral brand voice.]

## Requirements
- [Product A] version: X.X+ ([free or paid plan])
- [Product B] version: X.X+ ([free or paid plan])
- WordPress version: X.X+

## What This Integration Does
[Short bulleted list of what becomes possible with both products connected.]

## Setup

### Step 1: [Configure Product A]
[Full navigation path and steps]

### Step 2: [Configure Product B]
[Full navigation path and steps]

### Step 3: [Connect / Enable the Integration]
[How to activate the connection between the two products]

## Expected Outcome
[What the user should see when the integration is working correctly.]

## Common Use Cases
[2-3 concrete examples of what users can accomplish with this integration.]

## Notes or Limitations (Optional)

## Troubleshooting
[Link to troubleshooting doc or 2-3 most common issues inline]

## Related Docs
- [Link to Product A docs]
- [Link to Product B docs]
```

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
- When a feature requires a paid plan, call it out clearly at the top under Requirements — never buried in the middle.
- Use **bold** for UI labels exactly as they appear in the interface (e.g., **Save Changes**, **Enable**, **Typography**).
- Use `code formatting` for file paths, shortcodes, CSS snippets, filter/hook names, function names, and endpoint paths.

### Structure
- Use H2 for major sections, H3 for sub-sections. Never skip heading levels.
- Steps go in numbered lists. Options/settings go in bullet lists or tables.
- Group related settings together — don't list them in random order.
- Most common use case first. Edge cases go at the bottom or in a Notes section.
- Always include an **Expected Outcome** section after steps so users can confirm it worked.

### Version-Specific Content
When a product has major versions with meaningfully different UI or behavior (e.g., Spectra Legacy vs Spectra One), state at the top which version the doc applies to:

> **Note:** This doc applies to **Spectra One** (v2.0+). For the legacy editor, see [Spectra Legacy docs](https://wpspectra.com/docs/).

### Screenshots
- Viewport: **1280×800px** (set via browser dev tools).
- Clean WordPress install — only required plugins active, no unrelated plugins visible in menus or UI.
- Account name in screenshots: use **BSF Docs**, **SureCart Docs**, or **John Doe**. Never personal usernames.
- Always blur or remove: API keys, tokens, email addresses, account identifiers.
- Upload screenshots directly to WordPress — never embed from Google Docs or external hosts.
- Screenshots support the text, they don't replace it. Never write "as shown in the image" — the text must stand alone.
- If removing a screenshot doesn't reduce clarity, it's unnecessary.

### Media Placeholders
When screenshots or videos are needed, add a placeholder:
- `[Screenshot: Show location of X setting — WordPress Dashboard → Product → Tab]`
- `[Video: Walkthrough of setting up X from scratch]`

Don't skip these — they're reminders for the publishing step.

### Free vs Paid Callouts
Always be explicit. Use the **Pro Feature** callout at the top under Requirements, and again inline if only a specific step requires a paid plan. WebFetch the pricing URL to confirm current plan names before publishing.

> **Pro Feature:** This feature requires a paid plan. [See plans](PRICING_URL).

For free features:
> **Note:** This feature is available in the **free version** of [Product].

---

## URL Verification Rule

**Never add a URL to a doc without verifying it first.** This applies to all links — related docs, support pages, pricing pages, upgrade links, or any external reference.

Before including any link:
1. **WebFetch the URL** and confirm the page exists and contains the expected content.
2. If the page returns a 404, redirects somewhere unrelated, or doesn't exist — **do not include the link.** Use a placeholder instead: `[Link: page name — URL to be confirmed]`
3. Never construct a URL based on a pattern (e.g., assuming `/docs/feature-name/` exists just because similar URLs do).

This applies equally when **updating existing docs** — if a linked URL was added previously, verify it still resolves correctly before leaving it in.

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

1. **Identify the doc type** — feature guide, setup, troubleshooting, FAQ, developer reference, or integration guide.
2. **Confirm the single goal** — if there are multiple goals, split into separate docs.
3. **Ask for missing info** if the product, feature name, or context is unclear. Don't guess.
4. **Use the matching template** from above.
5. **Fill every section** — mark `[To be added]` only for optional sections, not required ones.
6. **Add screenshot/video placeholders** wherever media would help.
7. **WebFetch the pricing URL** if any paid plan mention is needed — confirm current plan names.
8. **Run the pre-publish checklist** before finalizing.

---

## Workflow: How to Update an Existing Doc

1. **Read the existing doc in full** before making any changes. Understand what it currently covers.
2. **Identify what's changing** — new steps, removed steps, updated UI labels, changed navigation paths, deprecated features, added requirements, or structural improvements.
3. **Do not rewrite what isn't broken.** Preserve working sections, existing examples, and screenshot placeholders unless they're directly affected by the change.
4. **Update section by section** — don't replace the whole doc unless a full rewrite is explicitly requested.
5. **Flag anything that needs a new screenshot** — if a UI path or setting has changed, add or update the screenshot placeholder.
6. **Check consistency** — after updating, verify that terminology is still consistent throughout the whole doc (not just the updated section).
7. **Run the pre-publish checklist** on the full doc, not just the changed parts.

---

## Pre-Publish Checklist

- [ ] Single clear goal — no mixed objectives
- [ ] Neutral brand voice (no "I", "we", no author name)
- [ ] No internal context exposed (no GitHub issues, Slack references, regression mentions, or internal trade-off language)
- [ ] Full navigation paths on every setting
- [ ] Free vs paid requirement stated at the top
- [ ] All steps numbered and actionable
- [ ] Expected Outcome section included
- [ ] UI labels bolded exactly as they appear in the interface
- [ ] Consistent terminology throughout (one term per concept)
- [ ] Screenshot placeholders added where needed
- [ ] No filler intro ("In this doc we will…")
- [ ] No marketing language or superlatives
- [ ] Notes/limitations section included if relevant
- [ ] All URLs verified — WebFetched and confirmed to exist with correct content (no guessed or assumed links)
- [ ] FAQ uses behavioral questions only (if included)
- [ ] Pricing page WebFetched and plan names confirmed (if any plan or tier is mentioned)
- [ ] Version callout added if doc applies to a specific product version (if relevant)
- [ ] Developer Reference: all code examples tested or marked [To be verified] (if doc type 5)
- [ ] Integration Guide: BSF products recommended first before third-party alternatives (if doc type 6)
